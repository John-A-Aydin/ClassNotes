Before you do something (disk writes) note down what you're going to do

If an oopsie happens you know what you were doing

## Data Journaling

When we update a file (appending a data block to a file), The following structures are updated
- inode
- bitmap
- data block

First we journal write: 
- Transaction Begin (TxB)
- Note down the inode, bitmap, datablock
	- This data can be LARGE
- Transaction End (TxE)
	- First write all blocks except TxE then once everything else is done write TxE
	- This gives us a binary written or not written status for each journal entry

