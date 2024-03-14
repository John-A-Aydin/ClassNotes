
```TypeScript
Set S
func find_leaves(node) : Set<Tree Node>
	if (node == null) return
	if (node.left == null && node.right == null) return S
	return find_leaves(node.left) + find_leaves(node.right)
```