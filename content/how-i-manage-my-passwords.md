+++
title = "How i manage my passwords"
date = 2019-06-30
draft = true
[taxonomies]
tags = ["passwords"]
+++

I can't remember a different password for every website.
So i decided to use a password manager. Instead of using a password manager that offers
syncing across devices, i decided to use [keepass xc](https://keepassxc.org), which stores the password database locally, encrypted.
While this is secure, i still needed to use the passwords on my phone.
Fortunately, there is [syncthing](https://syncthing.net), a program to sync files across two or more devices, without relying on a central
authority. It is p2p and encrypted, so no one can steal your password database.
On android i also installed the keepass dx (also called keepass deluxe) app to view my password database.

### Enabling two factor auth (2FA)

Must read:
[Getting 2FA right in 2019](https://blog.trailofbits.com/2019/06/20/getting-2fa-right-in-2019/)
[hn comments](https://news.ycombinator.com/item?id=20232164)

TL;DR for everyone:

2FA is a must have if you want to be secure online. You should keep your time-based one time passwords (TOTP)
separate from the other normal passwords, else it's useless. SMS verification is convenient but not as secure as TOTP codes
(but i gueess it's still better than nothing). Also you shouldn't use 2FA recovery codes to login normally,
but only in the case you have lost access to the TOTP codes.

If you don't know which app/program to use, i recommend the following ones:

- [Aegis (android)](https://github.com/beemdevelopment/Aegis)
- [Authenticator (GNU/linux)](https://gitlab.gnome.org/World/Authenticator)
