# Stack traces

Java stack traces are probably familiar to even those who do not program in Java, because when something goes
wrong inside a JVM application, frequently they show the raw stack trace on the output.

While the usefulness of a stack trace for a usual user is debatable, it is clear that this snippet of
text contains a lot of information about the problem and helps identifying the cause. However, a raw
stack trace is closer to machines than to humans, that's why we think [stack trace search](search/search.md) can help you.

## What is a stack trace

When an application throws an exception, the method call hierarchy of that execution thread will be
saved to the exception as an array of stack frames. The first stack frame is the current method, the
last stack frame is the start of the thread (e.g. Thread.run(), or the entry point of your application).

A Java stack trace is a textual representation of a thrown exception. While there is no standard format,
conventionally it look like this (read more in the [docs](https://docs.oracle.com/javase/8/docs/api/java/lang/Throwable.html#printStackTrace--)):
```
com.samebug.test.TestException
        at com.samebug.test.Test.fail(Test.java:25)
        at com.samebug.test.Test.main(Test.java:13)
Caused by: java.lang.NumberFormatException: For input string: "4f8:0:a102::add:9999"
        at java.lang.NumberFormatException.forInputString(NumberFormatException.java:48)
        at java.lang.Integer.parseInt(Integer.java:458)
        at java.lang.Integer.parseInt(Integer.java:499)
        at com.samebug.test.Test.fail(Test.java:23)
        ... 1 more
```

The important points here:
- The stack trace starts with the fully qualified name of the exception type.
- After the exception type, optionally there is an exception message.
- The stack frames contain the fully qualified name of the class and the method, and might contain the source location.
- The exception might have a 'cause', a lower level exception that was wrapped in the higher level
(in the above case, `java.lang.NumberFormatException` was wrapped in `com.samebug.test.TestException`).
- The line starting with `...` is part of the stack trace, it is just a shorthand to reduce the length of the output.
