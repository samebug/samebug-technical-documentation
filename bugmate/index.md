# Bugmates

When you [search](/guide/search) with a [stack trace](/guide/stack-trace), Samebug will show your bugmates along with other [solutions](/guide/solution).
Bugmates are actually [crash tags](/guide/solution/rating-solutions), Samebug users associated with stack traces.

## Rationale

Our rationale behind bugmates was the situation which is probably familiar to you: you have an exception,
you try to search for a solution on the Internet but find nothing. Probably there were already a number of other
developers struggling with the same problem who put some effort into solving it, managed to fix it but never
shared their findings. They left no trace, not even the fact that they had such a problem. We see exceptions
every day, but only a small portion of these crashes get documented by people who ask for a solution
on the forums.

![Bugmates](https://samebug.io/static/images/docs/bugmates.png)

Bugmates are Samebug's concept to improve this situation. Every stack trace search executed
on the web and every crash logged during development in the IDE (assuming the [Samebug plugin](/guide/integration/intellij-idea/install)
is installed) will be associated with the Samebug user. In some cases these people just ignore
the exception, others will find a workaround or put more or less effort into finding the solution,
but only in the rarest case will someone document the problem and the solution e.g. in a blog post.
However, because they use Samebug, their effort and knowledge is no longer isolated.

## Privacy

We know that the information that Samebug deals with might be sensitive, we have an
adequate idea about [privacy](/guide/privacy) even in this early phase.

In the context of bugmates these concepts translate to:

- If your searches are *Public*, other users can find you via bugmate match and read the stack trace of the crash you had.
- If your searches are *Searchable*, other users can find you via bugmate match, but will not see the stack trace of the crash you had.
- If your searches are *Private*, you will never show up as a bugmate for people who cannot access your workspace. This is only available in the paid version ([Private Package](/pricing))
