
## Overall Organization

We divide the disk into blocks (sector)
- One block is 4 KB
- Addressed from 0 to N - 1 (like arrays)
The OS always knows the root directory bc its the root of the tree

#### Data Region in File System
- reserve data region to store user data 
- File system has to track which data block comprise a file, the size the file, the owner, etc

#### Inode table
- Reserve some space for inode table
	- this holds an array of on disk inodes
	- We need to know if a spot that an inode table is referencing is valid
- Each Inode is referred to by an inode number
	- Like an index
- To check if an inode is valid we check the inode bitmap
- 

#### Allocation Structures
Bitmap
- Tracks whether inodes or data blocks are allocated or free
- Use Bitmap, each bit indicates free(0) or in-use(1)

#### Super Block
- Contains number of inodes, begin location of inode table, etc
- When mounting a file system, the OS will read the super block first


### How to allocate files and directorise

- Keep related stuff together
- Place Inodes on the same disk level as their files



#### SEER Trace

Log order in which files are accesses
Path difference: how far up the dir tree until you find the common ancestor