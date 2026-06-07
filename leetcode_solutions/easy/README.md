### Q-1) Given the root of a binary tree, return the inorder traversal of its nodes' values.
- [Binary Tree Inorder Traversal](https://leetcode.com/problems/binary-tree-inorder-traversal/description/)
- [Solution](solution.java)

### Explanation:
We need to write a code that performs an Inorder Traversal of a binary tree and returns the node values in a List<Integer>. For this, we'll use the concept of recursion. First, let us all know what is Inorder Traversal.

Inorder Traversal - An inorder traversal is a depth-first algorithm used to visit or list all the nodes in a tree data structure. For every node, it visits: Left → Root → Right.

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
### Q-2) Given the root of a binary tree, return the Preorder traversal of its nodes' values.
- [Binary Tree Preorder Traversal](https://leetcode.com/problems/binary-tree-preorder-traversal/description/)
- [Solution](solution.java)

### Explanation:
We need to write a code that performs an Preorder Traversal of a binary tree and returns the node values in a List<Integer>. For this, we'll use the concept of recursion. First, let us all know what is Preorder Traversal.

Preorder Traversal - An preorder traversal is a depth-first algorithm used to visit or list all the nodes in a tree data structure. For every node, it visits: Root → Left → Right.

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

3. Visit Current Node
list.add(root.val);
Add the current node's value to the list.

4. Traverse Left Subtree
list.addAll(inorderTraversal(root.left));
Recursively get all values from the left subtree and append them.

5. Traverse Right Subtree
list.addAll(inorderTraversal(root.right));
Recursively get values from the right subtree and append them.

6. Return Result
return list;
Return the inorder traversal of the current subtree.
```

### Q-3) Given the root of a binary tree, return the Postorder traversal of its nodes' values.
- [Binary Tree Postorder Traversal](https://leetcode.com/problems/binary-tree-postorder-traversal/description/)
- [Solution](solution.java)

### Explanation:
We need to write a code that performs an Postorder Traversal of a binary tree and returns the node values in a List<Integer>. For this, we'll use the concept of recursion. First, let us all know what is Inorder Traversal.

Postorder Traversal - An postorder traversal is a depth-first algorithm used to visit or list all the nodes in a tree data structure. For every node, it visits: Left → Right → Root.

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

4. Traverse Right Subtree
list.addAll(inorderTraversal(root.right));
Recursively get values from the right subtree and append them.

5. Visit Current Node
list.add(root.val);
Add the current node's value to the list.

6. Return Result
return list;
Return the inorder traversal of the current subtree.
```

