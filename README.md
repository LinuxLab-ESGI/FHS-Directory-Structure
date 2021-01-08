# FHS-Directory-Structure

A short abstract about FHS used by Linux distros.

Linux is essentially composed of directories et files but every directories have its utility. Whatever Linux distro you are using it is certainly using the FHS (**F**ilesytem **H**ierarchy **S**tandard). FHS defines the hierarchy and all the directorires to have for a GNU/Linux disto and Unix systems.

>A filesystem has two meaning which is generally clear from the context.
>The first meaning is the hierarchy of directories (directory tree) that is used to organize files on a computer system.
>The second meaning is the type of filesystem, it is how the storage of data is organized on the physical disk. Each type of filesystem has its own set of rules for controlling the allocation of disk space to files and for associating meta-data about each file with that file (filename, permissions, creation date, ...)
>Examples of filesystem : ext4, btrfs, xfs, ...

## Filesystem

The file system on Linux is organized like a **tree**. At the very top of the tree, there is the **root** wich contains folders that have a particular purpose.  
Any file path in the Linux system starts from the root. This root is noted with a slash **/**.

>This root could be compare to the **C:\\** of Windows.

## Paths

A **path** is the location of a folder from the root.
Moving from the root trough the folders is called When you start from the root and then move through the folders, the whole location is called path.  
There are 2 types of a path :

- **Absolute path**, which starts from the root : */home/user/docs/example* (the **pwd** command show your current path)

> This mean wherever we are located we can go to *example* by typing `cd */home/user/docs/example*`

- **Relative path**, which starts from the place where we are located. For example, if we are in */home/user*, the relative path to go to *example* is docs/example.

> This means we have to be in the parent folder to go to *example* by typing **cd docs/example**

## Main directories

Here are the main directories present in most distros :

| Directory | Utility                                                                                                        |
| --------- | -------------------------------------------------------------------------------------------------------------- |
| /         | Root directory of the entire filesystem                                                                        |
| /bin      | (**bin**aries) Essential binaries usable by every users                                                        |
| /boot     | Files for Linux startup (Bootloader, kernel, initrd, ...)                                                      |
| /dev      | (**dev**ice) Entry point for devices (scree, disks, partitions, null, TTY, webcam, ...)                        |
| /etc      | (**e**diting **t**ext **c**onfig) Files for services and system configurations                                 |
| /etc/opt  | (**opt**ional) Configuration files for additionnal programs and software stored in /opt                        |
| /home     | users' home directory for peronnal data and settings                                                           |
| /lib      | (**lib**raries) Libraries for all the binaries                                                                 |
| /media    | mounting point for removable devices (CD-ROMs)                                                                 |
| /mnt      | (**m**ou**nt**) Temporary mounting point for removable devices                                                     |
| /opt      | (**opt**ional) Additionnal softwares and programs installed out of the distro's repo                           |
| /proc     | (**proc**ess) Vitual directory containing informations about the kernel and process                            |
| /root     | Home directory of the user root                                                                                |
| /run      | (**run**tim system) Files about the running system  (executed services and users informations)                 |
| /sbin     | (**s**uper **bin**aries)                                                                                       |
| /srv      | (**s**e**rv**ices) Essential binaries only usable by root user (usually system binaries)                       |
| /sys      | (**sys**tem) Inforamtion about devices, drivers and kernels features                                           |
| /tmp      | (**t**e**mp**orary) Directory to store temporary files for users and system (cleared after a reboot)           |
| /usr      | (**u**nix **s**ystem **r**essources) Binaries, documentation, source code, libraries for second level program. |
| /var      | (**var**iables) logs, databases, web sites, ...                                                                |

___
Updated : 08/01/2021
Author : AnthonyF
