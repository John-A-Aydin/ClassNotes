### In order traversal of a binary tree
``` Python
func inorder(node)
	if node != null
		inorder(node.left)
		print(node)
		inorder(node.right)
```
