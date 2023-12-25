
tries to make everything sequential


Just writes the new block and updates the metadata late,

**Write buffering**

# Main Idea

When we update a file, we also have to update the inode

LFS just buffers the heck out of the data and when it gets full up it just dumps them on the drive 

### Trade-offs
LFS only benifits a bunch of small writes


### Checkpoint Region
Fixed location in the LFS partition
Contains the pointers to the latest of the inode map

### [[Fragmentation]]
LFS does not deal with disk fragmentation
- If we wanted to eliminate fragmentation we'd have to load the entire file into mem and then write out the entire file after modifications
### Garbage
LFS just leaves older versions of the file all over the disk

##### Overwrite
Both the inode and data blocks are turned into garbage

##### Append
A new inode is created that points to the old data block
- Old inode is now garbage

##### Garbage Collection
Periodically cleans the older versions of file data

Which blocks to consolidate
- Hot Segments
	- Clean later
- Cold Segments
	- Clean now??



# Study guide

What is the inode map?


Why does LFS have it when FFS and earlier file systems didn't?

What makes LFS faster
	write buffering to make large sequential writes

Does LFS prevent fragmentation
	No

Why does LFS have two checkpoint regions
	If were writing out to the checkpoint and the computer dies we need a backup.

What is stored in the checkpoint region *
	Location of inode map

Why does LFS have garbage collection?
	
==Check link on actual study guide==
