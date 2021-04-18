# Challenge Accepted 8


[101. 对称二叉树](https://leetcode-cn.com/problems/symmetric-tree/)

![](图片地址)

### 方法一：递归

```java
func isSymmetric(root *TreeNode) bool {
	return check(root, root)
}
func check(p, q *TreeNode) bool {
	if p == nil && q == nil {
		return true
	}
	if p == nil || q == nil {
		return false
	}
	return p.Val == q.Val && check(p.Left, q.Right) && check(p.Right, q.Left)
}
```
g