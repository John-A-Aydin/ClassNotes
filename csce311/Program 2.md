Spin up ur own threads in the internal logic

Make sure you lock your stuff

### Idea using hash table
| put          | lookup                 | remove |
| ------------ | ---------------------- | ------ |
| sem val of 1 | sem val == num threads | sem val of 1?       |
	

## Idea using BST

async traversal, locked modification

would need to hande cases where thread finds value and it is deleted while its waiting



