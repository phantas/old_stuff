It was my main intent here to write a script that would allow me to daily create backups of critical data and sync it to a remote location for storage. Since I would be using a internet provider for the remote location instead of a privately owned server, I wanted the remote copy to be encrypted at all times and to do this efficiently, both in terms of time and communication.

This package contains 2 files

 * backup - a shell script that generates basic tarball backups of files.
            Optionally burns the backups to a DVD or syncs to a remote location
            or device (not encrypted).

 * dailybackup - a shell script that securely backups critical files by breaking
                 into blocks and encrypting via PGP. if a local encrypted copy is kept
                 only the files that have been altered are updated.
                 Optionally syncs to a remote location. 
 
                 Since the encryption is done locally and only the altered files 
                 are repacked and encrypted, communication is minimised and at no
                 point is the data present in plain form in the remote location.
