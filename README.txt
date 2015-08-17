GARBAGE COMPACTOR

Garbage compactor is a prototype for a tool for deleting
files. Instead of fully deleting them, it moves them to
~/.gc, changes their name to the Unix time stap at removal
time and compresses them. A log will be kept so deleted
files can be restored almost easily.

As said this is a prototype that will be made more user
friendly in the future. Patches and pull requests are
more than wellcome.

Garbage compactor is free software distributes under the
MIT license.

INSTALLATION

cp ./gc /usr/bin

USAGE

To delete a file

gc d [file name]

To view a deleted file

gc p [Unix time stamp of deletion time (see the log)]

To restore a file

gc r [Unix time stamp of deletion time (see the log)]

To view the log

gc l

To empty the log and permanently remove all deleted files

gc empty

TO DO

-Dirrectory support
