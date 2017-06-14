# Samebug search

By searching with a [stack trace](stack-trace.md) Samebug can provide you a more relevant [solution](solutions.md)
to your software crashes. You don’t have to browse through endless forums and developer communities.

## How to use Samebug search with a stack trace

When you need help for a stack trace, just copy the text of the stack trace and paste it to [Samebug](https://samebug.io/search).
However, please be careful to copy the full text of the stack trace, and include every character
from the beginning of the exception type until the very end of the last 'Caused by' clause if there is any. A few
missing characters can dramatically change the meaning of the stack trace and Samebug has no means to recognize
if you made a mistake or did that on purpose.

To save you from this hassle we created the Samebug plugin for
[IntelliJ Idea](integration/intellij-idea/install.md) and
[Android Studio](integration/android-studio/install.md),
which integrates Samebug to your development workflow by bringing stack trace search right where you need,
one click away at the console of your IDE.

## Why use Samebug search with a stack trace

If you paste an arbitrary text to the search area of Samebug which can't be parsed as a [valid stack trace](stack-trace.md),
Samebug will fall back to text search mode. In many cases this might be still good enough for you, but
using stack trace search will always produce more relevant results. Only when you paste a valid stack trace,
can Samebug analyze the semantics of the stack trace and use our unique stack trace similarity algorithm.
