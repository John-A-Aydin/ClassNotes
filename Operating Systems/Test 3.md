NO SECURITY!!!!!!!!
# Ch 36

#### Polling
- OS queries for changes
- simple
- a lot of "nothing to be done"

#### Interrupts
- OS is notified when work/events happen
- act like traps

#### DMA
- Direct Memory Access
- Handle large mem requests and interrupt when done
- Minimizes work on CPU

#### Drivers
- Software that allows hardware to interact with OS

#  Ch 37

#### Basic Geometry
- Track, Cylinder, Platter, Rotation

#### Costs
- See slide 10 formula
- Rotation Delay
	- Time for disk to rotate to piece of data under the head after the head gets to the right track
- Seek Time
	- Time to move head from track to track

#### Random vs. Sequential Access
- Random sucks fr

#### Track Buffer
- Because of rotation and spatial locality, likely to need data under head in the future

#### Disk Scheduling Questions
- ????

## Ch 38

#### Raid levels
[[RAID]]
Reliability and/or Speed
- RAID 0: 
	- Striping
- RAID 1:
	- Mirroring
- RAID 4:
	- Add one parity disk instead of mirroring
	- Bottlenecks with many small writes
 - RAID 5: 
	 - RAID 4, where you stripe the parity disk

#### Parity

## Ch 39

#### Inode vs "file" vs Directory

## Ch 40

#### Block, Chunks


#### Block Group vs Cylinder Group
- Nowadays the cpu is told the block group (array like)
- Back then the cpu could see the Cylnder

#### Basic File System Data Structures
- Super Block
	- Contains general file system info
	- Big ol array
- Bitmaps
	- Boolean array
	- Tells us whether an inode is valid
- Inode Blocks
	- Logically an array of Inodes
- Data

#### Indexed Allocation
- Direct, single, double, and triple inderect

#### Steps to read or append to file
Lec 40 slide 14
1. Get there
	1. go to root node
	2. read the file inode
	3. read the bitmap
	4. ...

## Ch 41

#### Why is FFS Fast?
1. Keeps close files in the file system tree close together on disk
2. Spreads FS info across disk

#### (De)fragmentation
- Fragmentation is when blocks spread out over HDD
	- A lot of seek times
- Defragmentation
	- Get all them blocks together


## Ch 42

#### [[File System Checker (fsck)]]
- Looks around and fixes stuff

#### [[Journaling]]
- Write down all disk operations before doing it

See Lec 16 slide 5 (Guarenteed 1 question from this slide)


## NO Ch 43


## Ch 44
#### Wear leveling
- Deteriorate with more and more writes
- Cold Blocks
	- Files that never see writes
- Hot Blocks
	- Files that get written frequently


#### FTL

