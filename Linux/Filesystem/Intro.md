### Filesystem Hierarchy Standard (FHS)

The Filesystem Hierarchy Standard (FHS) specifies the standard directories and their contents for use with a filesystem. Here's a summarized table of the most important directories in the FHS, along with their purposes:

| **Directory**       | **Purpose**                                                          |
|---------------------|----------------------------------------------------------------------|
| `/`                  | The root of the primary filesystem hierarchy.                        |
| `/bin`               | Contains essential user binary executables.                         |
| `/boot`              | Contains the kernel and bootloader files.                           |
| `/dev`               | Populated with files representing attached devices.                  |
| `/etc`               | Configuration files specific to the host.                           |
| `/home`              | Common location for user home directories.                          |
| `/lib`               | Essential libraries to support `/bin` and `/sbin` executables.     |
| `/mnt`               | Mount point for temporarily mounting a filesystem.                  |
| `/opt`               | Optional third-party add-on software.                                |
| `/root`              | Home directory for the root user.                                   |
| `/sbin`              | Contains system or administrative binary executables.                |
| `/srv`               | May contain data provided by system services.                       |
| `/tmp`               | Location for creating temporary files.                               |
| `/usr`               | The root of the secondary filesystem hierarchy.                     |
| `/usr/bin`          | Contains the majority of the user commands.                         |
| `/usr/include`      | Header files for compiling C-based software.                        |
| `/usr/lib`          | Shared libraries to support `/usr/bin` and `/usr/sbin`.            |
| `/usr/local`        | The root of the third filesystem hierarchy for local software.      |
| `/usr/sbin`         | Non-vital system or administrative executables.                     |
| `/usr/share`        | Location for architecturally-independent data files.               |
| `/usr/share/dict`   | Word lists.                                                         |
| `/usr/share/doc`    | Documentation for software packages.                                 |
| `/usr/share/info`   | Information pages for software packages.                             |
| `/usr/share/locale` | Locale information.                                                 |
| `/usr/share/man`    | Location for man pages.                                             |
| `/usr/share/nls`    | Native language support files.                                      |
| `/run`              | Contains volatile data that changes at runtime (emerging standard). |
| `/sys`              | Mounts the sysfs pseudo-filesystem; exports information about kernel objects. |


Folders in FHS can be:

- shareable
- static
- variable: volatiles