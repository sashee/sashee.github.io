---
layout: post
title:  "Symlinks in Windows"
---

Symlinks are widely used in the Linux world. They offer an easy way to organise folders and
link things together. I didn't know they are available in Windows too.

Symlinks are like pointers. They reference something else, and whenever something needs the folder,
they are transparently redirected to the target. For example, you can have many Java installation,
and simply reference the selected one from a well-known place. This way it's easy and transparent
to switch between different versions.

You can also use a dotfiles repository and just reference your configurations. Then you have everything
in one place, easily transferable and savable. If you get in front of a new computer, just
clone and initialize your configurations and you can instantly feel like home.

The Windows terminology for symlinks are Junctures. They are effectively the same, they can be
created with some command line magic.

Why are they useful? I needed them to organize Dropbox-like backups. The problem is that I can not
move stuff into a single directory. There are installed software and organized documents that
must reside in a given place. On the other hand, Dropbox synchronizes from a single directory.

I could just copy all the stuff and let Dropbox save them. But that would defeat the whole purpose
of active synchronization. This would degrade the experience to the level of a snapshot-backup
system.

But symlinks made this possible. I simply link the directory, so that Dropbox is happy to see
all the files in its synch folder, while they actually remain at their original place.

One minor downside is the lack of write events. Dropbox picks up the changes in its directory,
but it apparently does not follow these links. But it synchronizes everything at startup, so
it only lags a little. Most of the changes will be backed up this way.

This opens the way to backup whole softwares with ease. Also it allows better organization
of folders; you don't need to put everything into one place. It's a nice way for peace of mind.

With the abundance of cloud synch services, you could easily constantly backup everything in your
computer without much hassle. No more excuses.
