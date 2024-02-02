![[Pasted image 20240129145157.png]]
> Unix * Originally Developed at Bell Labs 1969 * Thompson and Ritchie * Thompson created B language * Ritchie improved it and called it C * Unix rewritten in C « AT & T prevented from entering IT market * Couldn’t make a profit so let Unix out to universities at nominal cost

![[Pasted image 20240129145242.png]]
> * Became one of the most significant OS ever * Millions of copies shipped * Fast and Reliable * Even now 40 years on OS development is converging to Unix ideas * Unix with TCP/IP became the platform for Internet

* "Unix is light at the kernel level"
* "Does not do a huge amount, but does what it does efficiently"
## Timeline
---
![[Pasted image 20240129145225.png]]
> Timeline University of California produced BSD UNIX 1979 * AT & T now allowed to compete produced UNIX System V (became basis of ANSI STANDARD) in 1984 * 1989 AT & T produced SVR4 merged System V and BSD features * AT&T sold its Unix system laboratories to Novell 1993

## Examples of Unix
---
![[Pasted image 20240129145308.png]]
> + Company Unix System * USL (Novell) SVR4 * Sun SunOS HP HP-UX * Novell Unixware * IBM AlIX * DEC Ultrix * Redhat Software Linux * Apples latest OSX very Unix like

## Unix Architecture
---
![[Pasted image 20240129145522.png]]
> * The hardware is encapsulated by the kernel * It provides systems services to application programs * The user communicates with the kernel via the shell * The user can invoke the C compiler to create applications which can be executed by the kernel

![[Pasted image 20240129145540.png]]

## Unix File System
---
![[Pasted image 20240129150101.png]]
> * Hierarchical File Structure * All of the files in the UNIX file system are organized into a multi-leveled hierarchy called a directory tree. * A family tree is an example of a hierarchical structure that represents how the UNIX file system is organized. The UNIX file system might also be envisioned as an inverted tree or the root system of plant. * At the very top of the file system is single directory called "root" which is represented by a / (slash). All other files are "descendents" of root. * The number of levels is largely arbitrary, although most UNIX systems share some organizational similarities. |

![[Pasted image 20240129150116.png]]
> * i-nodes * A Unix file is described by an information block called an i-node. There is an i-node on disc for every file on the disc and there is also a copy in kernel memory for every open file. All the information about a file, other than it's name, is stored in the i-node. This information includes * File access and type information, collectively known as the mode. * File ownership information. * Time stamps for last modification, last access and last mode modification. * Link count. * File size in bytes. * Addresses of physical blocks.

![[Pasted image 20240129150129.png]]

![[Pasted image 20240129150141.png]]
> * There are 13 physical block addresses in an i-node, each of these addresses is 3 bytes long. * The first ten block addresses refer directly to data blocks, the next refers to a first level index block (which holds the addresses of further data blocks), the next refers to a second level index block (which holds the addresses of further index blocks) and the last refers to a third level index block (which holds the addresses of further second level index blocks). * All physical addresses associated with a file are implicitly assumed to reside on the same disc, there is no facility whereby a file could span more than one disc.

## When a Unix file is opened
---
![[Pasted image 20240129150213.png]]
> * Once a file has been opened the in-memory (the phrase "in-core" is traditionally used) version of the i-node contains significant extra information. This extra information includes * In-core i-node status indicating whether — the i-node is locked — a process is waiting for the i-node to be unlocked — the in-core i-node is dirty, i.e. differs from the disc version — file modifications have been made that haven't been written to disc * The device number of the disc the file belongs to. * The i-node number sometimes known as the i-number. On disc the i-nodes form an array and the i-number is inferred from the i-node's position in this array. * Pointers to other in-core i-nodes. * Areference count indicating the number of instances of the file being active or open.

## I node
---
![[Pasted image 20240129150247.png]]
> * In computing, an inode is a data structure on a traditional Unix-style file system such as ext2. An inode stores basic information about a regular file, directory, or other file system object. * When a file system is created, data structures that contain information about files are created. Each file has an inode and is identified by an inode number (i-number) in the file system where it resides. inodes store information on files such as user and group ownership, access mode (read, write, execute permissions) and type of file. There is a fixed number of inodes, which indicates the maximum number of files each filesystem can hold. * Afile's inode number can be found using the Is -i command, while the Is -l command will retrieve inode information

![[Pasted image 20240129150303.png]]
> * The POSIX standard mandates filesystem behavior that is strongly influenced by traditional UNIX filesystems. Regular files are required to have the following attributes: * The length of the file in bytes. * Device ID (this identifies the device containing the file). * The User ID of the file's owner. * The Group ID of the file. * Aninode number that identifies the file within the filesystem. * The file mode, which determines what users can read, write, and execute the file. * Timestamps telling when the inode itself was last changed (ctime), the file content last modified (mtime), and last accessed (atime). * A reference count telling how many hard links point to the inode

## Access Permission for Unix Files
---
![[Pasted image 20240129150334.png]]
> * UNIX is a multi-user system. Every file and directory in your account can be protected from or made accessible to other users by changing its access permissions. Every user has responsibility for controlling access to their files. * Permissions for a file or directory may be any or all of: * r-read * W -write * X -execute = running a program * Each permission (rwx) can be controlled at three levels: * U -user =yourself * g -group = can be people in the same project * o -other = everyone on the system

## Displaying File Access Permissions
---
![[Pasted image 20240129150359.png]]
> * File access permissions are displayed using the Is -l command. The output from the Is -| command shows all permissions for all levels as three groups of three according to the scheme: * owner read (r) owner write (w) owner execute (x) * group read (r) group write (w) group execute (x) * public read (r) public write (w) public execute (x) which are displayed as: -rwxrwxrwx

## Access Permissions with Chmod
---
![[Pasted image 20240129150441.png]]
> * The chmod command is used to change access permissions for files which you own. . Trtle syntax is: chmod permission_triads filename [who][action][permissions] where: * who action permissions * u=user *+=add r =read * g=group - = remove w = write * o =other X = execute - a=all * Examples: chmod a+r sample.f — Adds read permission for all users to the file sample.f. * chmod o-r sample.f - Removes read permission for others to the file sample.f. * chmod og+rx prog* - Adds read and execute permissions for group and others to all files which contain "prog” as the first four characters of their name. * chmod +w * - Adds write permission for user to all files in current directory.

### Numerical Method
---
![[Pasted image 20240129150510.png]]
> » File access permissions can also be changed by a numerical (octal) chmod specification. * Read permission is given the value 4, write permission the value 2 and execute permission 1. * rwx421 * These values are added together for any one user category: * 0=no permissions 1 = execute only 2 = write only » 3 = write and execute (1+2) * 4 =read only 5 = read and execute (4+1) 6 = read and write (4+2) 7 = read and write and execute (4+2+1) * So access permissions can be expressed as three digits. For example: » user group others * chmod 640 file1 rw- r-- --- * chmod 754 file1 rwx r-x r- * chmod 664 file1 rw- rw- r--

