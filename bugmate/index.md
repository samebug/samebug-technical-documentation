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

## Asking bugmates

Currently if you have an exception and check it on Samebug, even if it doesn't have a solution,
you might find your bugmates there, and you can send them a [help request](/guide/help-requests).

A help request is a stack trace and the description of the problem. The description might be
helpful for your bugmates to identify the problem in cases when the stack trace is not enough,
but you can leave it empty if you want.

When you send a help request, Samebug will notify your bugmates about it, and when they answer,
Samebug will notify you. We think from this procedure everybody profits:

- The bugmates did not have to write solutions in advance. Developers have lots of crashes, it
is not realistic to expect them to write and publish the solution for all of them
- You don't have to dig deep into a library looking for a problem that other people have already solved
- The bugmates won't be spammed with irrelevant help requests, they see only those where the
stack trace match suggests they can help
- When you mark the solution as helpful, you boost the author's [profile](/guide/profile)

## Cancel help request

If you are no longer interested in answers to your help request, you can revoke it on the same
page where you requested it. Right now it does not happen automatically even if you mark
one of the answers helpful.

## Privacy

We know that the information that Samebug deals with might be sensitive, we have an
adequate idea about [privacy](/guide/privacy) even in this early phase.

In the context of bugmates these concepts translate to:

- If your searches are *Public*, other users can find you via bugmate match and read the stack trace of the crash you had.
- If your searches are *Searchable*, other users can find you via bugmate match, but will not see the stack trace of the crash you had.
- If your searches are *Private*, you will never show up as a bugmate for people who cannot access your workspace.
