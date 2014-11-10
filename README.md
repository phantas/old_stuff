old_stuff
=========

Migrating some old stuff from personal page:

---------------------

# Hacks and Hobby projects.

_All of the below is provided as is, use it at your own risk._

* **ljfriends.pl** - LiveJournal provides feeds for individual journals but not to a user's friends page. This Perl script generates a RSS feed for said page.

** Requires: a paid, permanent or early adopter account, unfortunately... and a working installation of the Perl module HTML::Tidy (you may run into problems here)

** Warning: this script is not endorsed by LiveJournal and is provided as is. In particular, do not make the script usable publicly in a server- there is a security loophole that may be used to hang or crash your script/server.

* **secure_backup** - with the popularity of web services and remote locations, I have recently been playing with the idea of securely keeping remote backups of data. It is still very much in a conceptual stage ( I have also heard of some recent applications that appear to target at this, I haven't looked at them properly).

In the meantime, this package includes a hack shell script that does the job. It efficiently and securely packs and syncs data to a remote location. Only altered chunks of data are repacked and synced and data is never present in an unencrypted form other than locally - the data is already encrypted when synced. However, it does not yet provide an interface to recover the data from the backups (for now, it must be done "by hand").
The typical backup to tarballs script is also included.

* euro.pl - if you play EuroMillions aka Lotto, this little Perl script checks combinations against the winning combination (fetched on the background) and even gives an estimate to the prize if one is eligible. Yes, I'll translate it to English at some point.
