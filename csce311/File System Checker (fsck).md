#### fsck is a Unix tool for finding inconsistencies and repairing them.
- super block: if the number of blocks in the filesystem is larger than the filesystem size (and other sanity checks)
- free blocks: find all the blocks accessible from the root directory and see if it matches the block bitmap.
- inode state: check if the state of each inode is valid
- inode link: check if the reference count for each inode is consistent
- check if a block is shared by two inodes.
- check for “bad” block pointer: ”bad” block pointer is the one that points to the location that lies outside the filesystem partition.
- directory: Check if . and .. are properly set up. Make sure that there are only one hardlink for a directory. 

Can take a very long time bc it goes over a whole disk