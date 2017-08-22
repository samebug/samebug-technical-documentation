# Privacy

We know that privacy can be an issue when dealing with stack traces. The stack trace tells information about the technology stack you use, the internal architecture of your modules, and the message can contain schema of your database tables, user names or worse. If your business consider these data sensitive, Samebug is ready to handle them respectively.

For every content you create on Samebug (at the moment there are crashes and solutions), you can specify three visibility level: *Public*, *Searchable* and *Private*.

- **Public** means that you don't consider this content sensitive. It's available openly on the Internet, anybody can access it.
- **Private** is exactly the opposite, only those Samebug users can access it who are granted permission by you. Others won't even know it exists.
- **Searchable** is a fine middle ground between being totally open or close. Broadly it means that your stack trace is private, but the content attached to it is public.

## Detailed explanation

At the moment there are two kind of data you create on Samebug: crashes and solutions.

Crashes are the stack trace searches you paste on the site or you submit from the [IDE plugins](/guide/integration/intellij-idea/install). If your search is *Public*, everybody will be able to check the stack trace of the crash, find you as a [bugmate](/guide/bugmate) for similar stack traces and your experience with the related libraries will be displayed on your [profile](/guide/profile). On *Private* level, none of these will be visible for unprivileged users, while on *Searchable* your stack trace will be private, but the rest of the data is public.

![](https://samebug.io/static/images/docs//samebug-privacy-you.png "Effect of privacy levels on your searches")

Solutions are the [tips](/guide/write-tip) you can attach to stack traces. If your solution is *Public*, everybody will be able to check the stack trace you wrote the tip for, the tip itself and your experience with the related libraries will be displayed on your [profile](/guide/profile). On *Private* level, none of these will be visible for unprivileged users, while on *Searchable* your stack trace will be private, but your tip and your experience is public.

![](https://samebug.io/static/images/docs//samebug-privacy-tip.png "Effect of privacy levels on your tips")

## How to set the visibility of your content

Any content you create will inherit the visibility of the [workspace](/guide/workspace) where it was created.
Changing the visibility of a single content is not possible currently; in case you want to do this please [contact us](mailto:hello@samebug.io)

## Which visibility level to use

Chosing which visibility level you should use depends on your situation. The more open you are, the more you give to the Community, and the less compensation we ask.

- **Public**: This is great if you are learning, exploring a new library, working on your pet project or doing open source development. Your stack traces are available for everybody. This is the default for unregistered Samebug users.
- **Searchable**: You should choose this level if you fear that sensitive information might leak into the exception message of your stack traces, but you don't mind if others know what kind of applications are you developing. People will see your journey, know the libraries you have experience with. When an other developer search with a stack trace similar to one that you saw, they can ask you for help, but Samebug will only show them the matching stack frames, neither the ones unique to you nor the exception message. This is the default for registered Samebug users.
- **Private**: You should consider this level if you think that any information about your development is an attack vector on you or your company. On private visibility you contribute nothing to the Community. This is available for enterprise users only.
