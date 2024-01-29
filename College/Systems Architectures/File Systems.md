![[Pasted image 20240129144933.png]]
> File Systems * File Organization * Creation Deletion Modification * Privileged Access * Protection * Encryption

## What is a file?
---
![[Pasted image 20240129145603.png]]
> * File is a named persistent collection of data * Unstructured, sequential (UNIX) — Data is accessed by specifying the offset * Collection of records (database systems) — Supports associative access » give me all records with “Name=Yossi” Attributes: owner, permissions, modification time, size, etc...

## File Attributes
---
![[Pasted image 20240129145628.png]]
> * Name - only information kept in human-readable form * ldentifier — unique tag (number) identifies file within file system * Type — needed for systems that support different types * Location — pointer to file location on device * Size - current file size * Protection — controls who can do reading, writing, executing * Time, date, and user identification — data for protection, security, and usage monitoring * Information about files are kept in the directory structure, which is maintained on the disk

## Directories
---
![[Pasted image 20240129145654.png]]
> * Files are Kept in Directories which are logical groupings of files. * The advantages of Directory Structures are: * Efficiency — locating a file quickly * Naming — convenient to users — Two users can have same name for different files — The same file can have several different names * Grouping — logical grouping of files by properties

## What can be done with files?
---
![[Pasted image 20240129145729.png]]
> » Search for a file * Create afile * Delete a file * List a directory * Rename a file * Traverse the file system

![[Pasted image 20240129145743.png]]
> * File data access — READ: Bring a specified chunk of data from file into the process virtual address space — WRITE: Write a specified chunk of data from the process virtual address space to the file * CREATE, DELETE, SEEK, TRUNCATE * open, close, set_attributes

![[Pasted image 20240129145759.png]]
> * Several pieces of data are needed to manage open files: — File pointer: pointer to last read/write location, per process that has the file open — File-open count: counter of number of times a file is open — to allow removal of data from open-file table when last processes closes it — Disk location of the file: cache of data access information — Access rights: per-process access mode information

## How do we access files?
---
![[Pasted image 20240129145830.png]]
> * A control structure, File Control Block (FCB), is associated with each file in the file system — Each FCB has a unique identifier (FCB ID) — UNIX: i-node, identified by i-node number * FCB structure: — File attributes — A data structure for accessing the file’s data

![[Pasted image 20240129145847.png]]
> » Given the file name » Get to the file’s FCB using the file system catalog + Use the FCB to get to the desired offset within the file data * The catalog maps a file name to the FCB — Checks permissions * This can be done for each file data access — Inefficient: Do this once when the file is first referenced * file_handle=open(file_name): — search the catalog and bring FCB into the memory — UNIX: in-memory FCB: in-core i-node » close(file_handle): release FCB from memory

## Contiguous Blocks Method
---
![[Pasted image 20240129145917.png]]

![[Pasted image 20240129145929.png]]
> * «In this approach, each file occupies a set of contiguous * blocks on the disk. * «Simple -- only starting location (block #) and length * (number of blocks) are required. * Random access * Wasteful of space (dynamic storage- allocation problem) * First-Fit and Best-Fit are common approaches * <Files cannot grow (variation exist)

## Linked Allocation
---
![[Pasted image 20240129145949.png]]
> * eIn this approach, each file is a * linked list of disk blocks; blocks * may be scattered anywhere on the * disk * +Allocate as needed, link together * <Example: File starts at block 9 » «Simple: need only starting * address * +Free-space management system -- * no waste of space * +Norandom access

## Index Table Method
---
![[Pasted image 20240129150008.png]]

## File Allocation Table
---
![[Pasted image 20240129150025.png]]