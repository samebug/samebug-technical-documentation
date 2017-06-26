# Experimental features

Samebug does not handle stack traces as plain text, but has a deep understanding on them;
knows about exception type hierarchies, chained exceptions, generated codes and third party libraries.
During our research we noted that having information about which stack frames belong which
third party component not only made our stack trace similarity metrics better, but also
gave us some really exciting oppurtinities. While this is not our main focus now, we still
want to show this interesting dataset and give you an idea about our future plans with this.

## Explore, crash statistics

Have you ever been in a situation where you had to evaluate open source alternatives of a library?
You check the features they offer, take a look at the speed of development and support,
check their issues on github. Samebug crash statistics could be a valuable addition in
these cases, showing thing like:

- how many users had crash using this library
- how many different kind of exceptions originated from this library
- which methods produce the most exceptions
- can you find tips or other support for these exceptions

You can see a prototype of this idea at [explore](https://samebug.io/explore). We show a list
of third party components, and you can dig deeper by checking their packages, classes, methods,
and at last it shows the list of exceptions ever thrown by (or passed through) this method. Now
click on an exception type to see the cases where this method has thrown that exception.

Currently this service does not uses the searches of our users, it uses only the stack traces
we found on the Internet.

## Forecast, crash prevention

Even when experts make beginner's mistake when they start using a fresh library. Wouldn't it
be nice if Samebug could warn you when you are using a method that caused headache for other users?
Samebug does have a concept about which methods are problematic in this sense. If you
use the IDE plugin, Samebug could detect usage of such methods and show you some tips in advance.

## Library vendor support

Libraries are often underdocumented, not ergonomic, have not intuitive interfaces or unexpected behaviors.
In many cases this happens not only due to the lack of time but due to the lack of feedback from
the library users.

We think that this situation could be improved by Samebug: e.g. if we find that a particular
method frequently throws NullPointerException, the vendor might consider improving the documentation
of that method by emphasizing that some parameters are expected not to be `null`.

## Improve JavaDoc

We all know that the documentation of most libraries is far from perfect which can lead to
a lot of annoyances. Samebug could easily notice cases when a method frequently throws an
exception type that is not documented in its JavaDoc.
