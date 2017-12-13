# Rating solutions

The [Samebug search](/guide/search) algorithm uses the semantics of the [stack traces](/guide/stack-trace) to define similarity.
When it presents the [search results](/guide/solution), they are ordered by the similarity of the stack trace
of the solution. However, we do not automatically evaluate the content of the solution, so
we need the Community to rate them in order to make Samebug learn which solutions work.

## Mark as helpful

A tip before you upvote | A tip after you upvoted
:-------:|:-----------:
![](https://samebug.io/static/images/docs/tip.png) | ![](https://samebug.io/static/images/docs/tip-marked.png)

On the stack trace search result page you can press the upvote button on the solution
that you found worthy. This simple click has multiple effects:

- other Samebug users will see how helpful each solution is
- if the solution was a [tip](/guide/write-tip) written by a Samebug user, he will [get recognized](/guide/profile)
for writing helpful tips
- the Samebug search algorithm will have more information to weigh the value of the solutions
- a new [crash tag](/guide/solution/crash-tag) will be created, combining the stack trace you used to search and the content of the solution you marked
