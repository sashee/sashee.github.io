---
layout: post
title:  "Unmaintained software"
---

Software that is not actively developed is obsolete, by definition.
It might not seem like that at first, but once you try to use it,
you'll see.

Most people think of software like a table. If it's built and not apparently broken, it's good as
new. Why would a piece of code break? The same algorithms and the same logic is working.

The software is not something that works as-is. It needs an operating system, has some system
dependencies, and also uses various libraries. This makes it fragile. The routines are still
working the same as on the first day it went to production. But it might need a specific
software that is no longer maintained, or hard to keep running.

And you need to take the security aspect into consideration. Even a simple piece of code
is intricate if you consider its environment too. And obsolete software is vulnerable.

But if you want to update one piece, you'll soon realize you'll need to update everything. It's
like when you wanted to but a new PC a decade ago. If you wanted a new processor, you needed
a new motherboard too, because the socket was different. But a new motherboard meant
new RAM modules. And new video card, because that port is also changed every few years. Just
wanted a faster CPU, and bought a shiny new tower. And in two years, all was obsolete again.

Software is similar. You make a shiny Java app that works flawlessly with Maven and you are sure
it will continue to work until eternity. But a mere two years passed, and you see that the
next Maven is out, with some breaking changes. Then a new Java version, which does not support
your beloved Maven version. You need to migrate not only to a new Maven but to a new Java.
And these are just the surface. When you run an innocuous-looking
_mvn versions:display-dependency-updates_, you'll realize that nearly all the libraries are outdated too.
It started as a simple update, and you have a multi-days-long migration work.

The changing environment makes softwares obsolete, and not because the algorithms magically rust away.
You should embrace the notion that every piece of software brings maintenance burden.
