# myfilecmdmagic

By Jason Summers

https://github.com/jsummers/myfilecmdmagic

This project contains some experimental "magic" signature files for
the _file_ command, a Unix-centric file format identification utility.

To try these signatures: Assuming have a way to run _file_, run it
with the `-m` option. For example:

`$ file -m [...]/myfilecmdmagic/exe_magic example.exe`

These pattern files or subdirectories are designed to be used in
isolation. Integrating them into the main database (often found at
/usr/share/misc/magic or /etc/magic) may be difficult to do without
breaking things, and may be beyond the scope of this project.

For more information about the _file_ command:
* [File command website](https://www.darwinsys.com/file/)
* [Wikipedia article](https://en.wikipedia.org/wiki/File_%28command%29)
