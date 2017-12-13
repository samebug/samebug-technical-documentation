# Samebug tips

Tips are short solutions to an exception. They are limited in size (256 characters) because we want to give a solution quickly when you have problems with an exception. At the moment you 
will see them
- on the web, in the results of a stack trace search
- in the IDE plugin, when you open Samebug for a stack trace

## The goal of tips

The problem with exceptions during development is that they make you lose focus. Instead of developing
what you originally planned, you are now trying to understand this unexpected situation, browsing the
Internet, reading forums not even related to your problem, etc. The goal of tips is to minimize the
time you have to spend with these exceptions and get back to your workflow as soon as possible.

## Why should you write tips

When you have an exception from a third party library, usually it takes 5-30 minutes to understand
what happened and how you can fix it, while a tip reduces this time to 1-2 minutes. The reach of
a tip depends on the popularity of the library it helps with, e.g. if you write a good tip, it
may help hundreds of people every week.

On the other hand, writing tips is a way to improve your profile. Samebug shows the tips you write and the libraries where you solve problems on your profile page, so you can get recognized as an expert of a component.

## Where to write tips

Currently there are two ways to write a tip:

- *as a solution for your search*: If you search with a stack trace, at the bottom of the page you'll find a 'Write tip' button.
- *as a solution for an exception*: If you check an exception page, at the bottom of the page you'll find a 'Write tip' button.

## How to write a tip

When you write the tip, you have to write the actual message and optionally you can refer to a url as the source.

- The message must be longer than 5 characters and cannot be longer than 256 characters.
- Use markdown where necessary to highlight code fragments and urls. Use \` for quoting inline code and \`\`\` for quoting code blocks.
Refer to [Remarkable](https://jonschlinkert.github.io/remarkable/demo/) for more info.
- Be straightforward, clear and short.
- Do not try to explain the details of the situation, but think about what would've helped you the most when you got this exception for the first time.
- Do not cover multiple situations, rather write them as separate tips.

You should fill the source url only if the tip you wrote is an extract of a content from another site on the Internet. Please always give credit to the original authors by linking the specific answer:
 - on Stack Overflow, click the 'share' label under the answer and copy&paste that link
 - on GitHub, click on the time label on the top of the comment and copy&paste that link
 - on Google Groups, click the dropdown arrow on the top right of a comment and copy&paste the direct link

![Write tip](https://samebug.io/static/images/docs/write-tip.png)

## Privacy

We know that lots of information that Samebug deals with might be sensitive, we have an adequate idea about [privacy](/guide/privacy) even in this early phase.

In the context of tips written by you these concepts translate to:

- If your tip is **Public**, other users can find it via stack trace search and read the stack trace of the crash had.
- If your tip is **Searchable**, other users can find it via stack trace search, but will not see the stack trace of the crash you had.
- If your tip is **Private**, it will never show up for people who cannot access your workspace.
