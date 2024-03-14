```Python
func height(node)
	if (node == null) return -1
	return max(height(node.left), height(node.right)) + 1
```