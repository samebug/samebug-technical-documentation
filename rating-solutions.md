# Rating solutions

The Samebug search algorithm uses the semantics of the [stack traces](stacktrace.md) to define similarity.
When it presents the [search results](solutions.md), they are ordered by the similarity of the stack trace
of the solution. However, we do not automatically evaluate the content of the solution, so
we need the Community to rate them in order to make Samebug learn what are the good solutions.

## Mark as helpful

On the stack trace search result page you can press 'Mark as helpful' button on the solution
that you found worthy. This simple click has multiple effects:
- other Samebug users see the number of marks on each solution, and the more mark it has, the
more likely it contains some useful information
- if the solution was a [tip](write-tip.md) written by a Samebug user, he will get recognition for writing
helpful tips
- Samebug search algorithm will have more information to weigth the value of the solutions
- a new crash tag will be created combining the stack trace you used for search and the
 content of the solution you marked

## Crash tags

Usually we use the terms *solution* and *crash tag* interchangeably. 
A crash tag is a stack trace associated with a solution content, which can be anything
that helps solving that exception, like a website, a Stack Overflow answer, a tip, or even
 an other Samebug user. Actually when Samebug presents you results for a stack trace search,
it presents the crash tags stored in the Samebug database. 

In the previous section we mentioned that marking a solution helpful creates a new crash tag.
What does this exactly means? Suppose you are searching with the stack trace `S1`, and Samebug
shows a crash tag `S2 -> C` (stack trace `S2` associated with content `C`). Here if you mark
this solution helpful, you will create a new crash tag `S1 -> C`. This is important for two reasons:
- if someone searches with a stack trace that is more similar to `S1` than `S2`, Samebug can
offer the content `C` as a solution with higher relevancy
- the fresh crash tag is owned by you, so when it collect marks from other Samebug users,
these marks will boost your profile.


