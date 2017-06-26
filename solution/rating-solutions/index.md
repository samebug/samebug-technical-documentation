# Rating solutions

The [Samebug search](/docs/search) algorithm uses the semantics of the [stack traces](/docs/stack-trace) to define similarity.
When it presents the [search results](/docs/solution), they are ordered by the similarity of the stack trace
of the solution. However, we do not automatically evaluate the content of the solution, so
we need the Community to rate them in order to make Samebug learn what are the good solutions.

## Mark as helpful

A tip before you mark | A tip after you marked
:-------:|:-----------:
![](https://samebug.io/static/images/docs/tip.png) | ![](https://samebug.io/static/images/docs/tip-marked.png)

On the stack trace search result page you can press 'Mark as helpful' button on the solution
that you found worthy. This simple click has multiple effects:

- other Samebug users see the number of marks on each solution, and the more mark it has, the
more likely it contains some useful information
- if the solution was a [tip](/docs/write-tip) written by a Samebug user, he will [get recognition](/docs/profile)
for writing helpful tips
- Samebug search algorithm will have more information to weight the value of the solutions
- a new [crash tag](/docs/solution/crash-tag) will be created combining the stack trace you used for search and the content of the solution you marked
