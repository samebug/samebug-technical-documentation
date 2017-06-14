# Crash tag

Usually we use the terms *solution* and *crash tag* interchangeably.
A crash tag is a [stack trace](stack-trace.md) associated with a [solution content](solution.md), which can be anything
that helps solving that exception, like a website, a Stack Overflow answer, a tip, or even
an other Samebug user. Actually when Samebug presents you results for a [stack trace search](search.md),
it presents the crash tags stored in the Samebug database.

## Creating crash tags

In [rating solutions](rating-solutions.md) we mentioned that marking a solution helpful creates a new crash tag.
What does this exactly means? Suppose you are searching with the stack trace `S1`, and Samebug
shows a crash tag `S2 -> C` (stack trace `S2` associated with content `C`). Here if you mark
this solution helpful, you will create a new crash tag `S1 -> C`. This is important for two reasons:
- if someone searches with a stack trace that is more similar to `S1` than `S2`, Samebug can
offer the content `C` as a solution with higher relevancy
- the fresh crash tag is owned by you, so when it collect marks from other Samebug users,
these marks will boost your profile.

