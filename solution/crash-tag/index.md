# Crash tag

Usually we use the terms *solution* and *crash tag* interchangeably.
A crash tag is a [stack trace](/guide/stack-trace) associated with a [solution content](/guide/solution), which can be anything
that helps solving that exception, like a website, a Stack Overflow answer, a tip, or even
another Samebug user. Actually when Samebug presents you results for a [stack trace search](/guide/search),
it presents the crash tags stored in the Samebug database.

## Creating crash tags

In [rating solutions](/guide/solution/rating-solutions) we mentioned that marking a solution helpful creates a new crash tag.
What does this exactly mean? Suppose you are searching with the stack trace `S1`, and Samebug
shows a crash tag `S2 -> C` (stack trace `S2` associated with content `C`). Here if you mark
this solution helpful, you will create a new crash tag `S1 -> C`. This is important for two reasons:

- if someone searches with a stack trace that is more similar to `S1` than `S2`, Samebug can
offer the content `C` as a solution with higher relevancy
- the fresh crash tag is owned by you, so when it collect marks from other Samebug users,
these marks will boost your profile
