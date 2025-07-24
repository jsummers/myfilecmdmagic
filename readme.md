# myfilecmdmagic

By Jason Summers

https://github.com/jsummers/myfilecmdmagic

This project contains some experimental "magic" signature files for
the _file_ command, a Unix-centric file format identification utility.

To try these signatures: Assuming you have a way to run _file_, run it
with the `-m` option. For example:

`$ file -m [...]/myfilecmdmagic/exe_magic example.exe`

Alternatively, you can compile the patterns to .mgc format first.
There's a Makefile in the "mgc" subdirectory that creates a
compiled file "mgc/mfcm.mgc".

The patterns are intended to work with _file_ v5.44 and higher. They
might work as far back as v5.42.

These pattern files or subdirectories are designed to be used in
isolation. Integrating them into the main database (often found at
/usr/share/misc/magic or /etc/magic) may be difficult to do without
breaking things, and may be beyond the scope of this project.

Patterns in the "workshop" subdirectory are even more experimental
than the others. They may cause too many false positives, or need
more testing, or just not be very good, or have a special purpose,
or need a newer software version; or the format may be too rare or
out of scope.

For more information about the _file_ command:
* [File command website](https://www.darwinsys.com/file/)
* [Wikipedia article](https://en.wikipedia.org/wiki/File_%28command%29)
