# Samebug search

By searching with a [stack trace](/guide/stack-trace) Samebug can provide you a more relevant [solution](/guide/solution)
to your software crash. You don’t have to browse through endless forums and developer communities.

## How to use Samebug search with a stack trace

When you need help for a stack trace, just copy the text of the stack trace and paste it to [Samebug](https://samebug.io/search).
However, please be careful and copy the full text of the stack trace, and include every character
from the beginning of the exception type until the very end of the last 'Caused by' clause if there is any. A few missing characters can dramatically change the meaning of the stack trace and Samebug has no means to recognize if you made a mistake or did that on purpose.

To save you from this hassle we created the Samebug plugin for
[IntelliJ Idea](/guide/integration/intellij-idea/install),
[Android Studio](/guide/integration/android-studio/install) and [Eclipse](/guide/integration/eclipse),
which integrates Samebug with your development workflow by bringing stack trace search to right where you need it,
one click away in the console of your IDE.

## Why use Samebug search with a stack trace

If you paste an arbitrary text into the search area of Samebug which can't be parsed as a [valid stack trace](/guide/stack-trace),
Samebug will fall back to text search mode. In many cases this might be still good enough for you, but
using stack trace search will always produce more relevant results. Only when you paste a valid stack trace,
can Samebug analyze the semantics of the stack trace and use our unique stack trace similarity algorithm.

### Text search results

![](https://samebug.io/static/images/docs/text-search.png "Text search")

This is the result page when you search with the first line of a StringIndexOutOfBoundsException. As you can see, the first [tip](/guide/solution)
is silly, only the second is relevant. Also, there are more than ten thousand [external solutions](/guide/solution) (most of them are probably
not that helpful), and Samebug cannot connect you to [bugmates](/guide/bugmate).

### Stack trace search results

![](https://samebug.io/static/images/docs/stack-trace-search.png "Stack trace search")

However, when you search with the full stack trace of a StringIndexOutOfBoundsException, Samebug gives you this:

- Only one [tip](/guide/solution), but that one is relevant.
- Only a thousand [external solutions](/guide/solution), the rest were not good enough.
- Samebug knows 52 [bugmates](/guide/bugmate) with this problem, you can ask them for help.
