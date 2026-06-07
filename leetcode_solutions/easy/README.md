### Q-1) Given the root of a binary tree, return the inorder traversal of its nodes' values.
- [Binary Tree Inorder Traversal](https://leetcode.com/problems/binary-tree-inorder-traversal/description/)
- [Solution](solution.java)

### Explanation:
This code performs an Inorder Traversal of a binary tree using recursion and returns the node values in a List<Integer>.

Inorder Traversal - For every node, visit: Left → Root → Right.

**Approach-**
```java
1. Create a list 
List<Integer> list = new ArrayList<>();
This list will store the inorder traversal result for the current subtree.

2. Base Case - 
if(root == null){
    return list;
}
If the tree/subtree is empty(null), return an empty list. This stops the recursion.

3. Traverse Left Subtree
list.addAll(inorderTraversal(root.left));
Recursively get all values from the left subtree and add them to list.

4. Visit Current Node
list.add(root.val);
After finishing the left subtree, add the current node's value.

5. Traverse Right Subtree
list.addAll(inorderTraversal(root.right));
Recursively get values from the right subtree and append them.

6. Return Result
return list;
Return the inorder traversal of the current subtree.
```