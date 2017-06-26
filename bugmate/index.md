# Bugmates

When you [search](/docs/search) with a [stack trace](/docs/stack-trace), Samebug will show your bugmates along with other [solutions](/docs/solution).
Bugmates are actually [crash tags](/docs/solution/rating-solutions), Samebug users associated with stack traces.

## Rationale

Our rationale behind bugmates was the situation probably familiar to you: you have an exception,
try to search solution on the Internet and find nothing, while likely there was already a lot of other
developers struggling the same problem who put some effort to solve this problem, fixed it and never
shared it. They left no trace even about the fact that they had such a problem. We see exceptions
every day, but only a small portion of these crashes get documented by people who ask for solution
on forums.

![](https://samebug.io/static/docs/bugmates.png "Bugmates")

Bugmates are Samebug's concept to make this situation better. Every stack trace search executed
on the web and every crash logged during development in the IDE (assuming the [Samebug plugin](/docs/integration/intellij-idea/install)
is installed) will be associated with the Samebug user. In some cases these people just ignore
the exception, others will workaround it or put more or less time into finding the solution,
but only in the rarest case will someone document the problem and the solution e.g. in a blog post.
However, because they use Samebug, their effort and knowledge is no longer in isolation.

## Asking bugmates

Now if you have an exception and check it on Samebug, even if it doesn't have a solutions,
you might find your bugmates there, and you can send them a [help request](/docs/help-requests).

A help request is a stack trace and the description of the problem. The description might be
helpful for your bugmates to identify the problem in cases when the stack trace is not enough,
but you can leave it empty if you want.

When you send a help request, Samebug will notify your bugmates about it, and when they answer,
Samebug will notify you. We think in this procedure everybody profits:

- The bugmates did not have to write solutions in advance. Developers have lot of crashes, it
is not realistic to expect them to write and publish the solution for all of them
- You don't have to dig deep in a library looking for a problem that other people have already solved
- The bugmates won't be spammed with irrelevant help requests, they see only those where the
stack trace match suggests they can help.
- When you mark the solution as helpful, you boost the author's [profile](/docs/profile).

## Cancel help request

If you are no longer interested in answers to your help request, you can revoke it on the same
page where you requested it. At the moment it does not happen automatically even if you mark
one of the answers helpful.

## Privacy

We know that many information that Samebug deals with might be sensitive, we have an
adequate idea about [privacy](/docs/privacy) even in this early phase.

In the context of bugmates these concepts translate to:

- If your searches are *Public*, other users can find you via bugmate match, and read the stack trace of the crash had.
- If your searches are *Searchable*, other users can find you via bugmate match, but will not see the stack trace of the crash you had.
- If your searches are *Private*, you will never show up as a bugmate for people who cannot access your workspace.
