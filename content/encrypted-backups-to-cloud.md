+++
title = "Encrypted backups on cloud storage (and locally)"
date = 2019-07-02
draft = true
+++
There are [different backup solutions][0] you can use on GNU/Linux, but this is what i
am currently using:

I backup everything with [borg][1] to an external hdd.
Why borg? Because it encrypts everything and deduplicates the data. It is the best solution 
I've found which provides also these two important features.

### Backing everything up to cloud storage
To sync everything to cloud storage i am using [rclone][2] with the mega backend.
I chose mega because it provides a lot of free storage on the free plan (50gb), and it fast
compared to other solutions (eg. google drive is slow on rclone).

### "p2p" backups to trusted devices
I also use [syncthing][3] to sync folders from my pc to my phone.
Beware that when using syncthing the data is encrypted only during transmission,
so you have to be sure the device you are synching with is trusted, because it can read
your data.
I've also enabled versioning on my phone to save an old copy of a file when it's overwritten
on my pc.

### Automating everything
I automate my cloud backups using cron.d, by putting a script in the folder /etc/cron.daily/,
so that it get's executed daily.

[0]: https://wiki.archlinux.org/index.php/Synchronization_and_backup_programs
[1]: https://www.borgbackup.org/
[2]: https://rlcone.org
[3]: https://syncthing.net
