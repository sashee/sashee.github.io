---
layout: post
title:  "Ransomware"
---

Ransomware is one of the most irritating viruses. It encrypts the files it has access to and
demands money for the decryption keys. The most irritating part is that it is like a hard
drive failure: you realize that you should have a backup too late.

But ransomware is actually a bit worse than that. If you use a cloud-sync service like Dropbox,
then you are protected against hardware failure. Even if a meteor hits your laptop, your data
is safe and sound in the cloud. But a ransomware will overwrite those files too, and the Dropbox
client will happily upload them to the cloud; overwriting your existing files in the process.
You end up having the encrypted files backed up, but you still have no access to them.

Ransomware usually utilize asymmetric cryptography. There is a key that can encrypt,
and another one that can decrypt. Even if you reverse engineer the virus, you can not get the
decryption key. It might not be stored anywhere, but that's something you'll know if you pay.
Which you shouldn't btw.

So Dropbox will be no use. But there are traditional backup utilities that will help you. You can
zip your most precious data and upload it to somewhere manually, without synchronization utilities.
This way the encrypted files will not overwrite the originals automatically.

Or you can use cloud providers to store your data instead of your own computer. The Chromebook does this,
and it should be enough most of the time. If everything you do is in the cloud, losing your
laptop will merely be an irritation. Depending on your habits, it might be a viable alternative.
