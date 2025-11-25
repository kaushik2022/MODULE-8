# Ex.No:5
# Ex.Name : Write a C++ Functions to perform inorder,preorder and postorder traversal of the below given tree
## Date: 25/09/2025
## Aim:
To write C++ functions to perform inorder, preorder, and postorder traversals on a given binary tree.
## Algorithm:
```
1. Inorder Traversal Algorithm (Left → Root → Right)

Start the function.

If the root is NULL, return.

Traverse the left subtree recursively.

Print the root node.

Traverse the right subtree recursively.

End the function.

2. Preorder Traversal Algorithm (Root → Left → Right)

Start the function.

If the root is NULL, return.

Print the root node.

Traverse the left subtree recursively.

Traverse the right subtree recursively.

End the function.

3. Postorder Traversal Algorithm (Left → Right → Root)

Start the function.

If the root is NULL, return.

Traverse the left subtree recursively.

Traverse the right subtree recursively.

Print the root node.

End the function.

```
## Program:
```cpp
// Traverse Preorder
void traversePreOrder(struct node *temp) {
  if (temp != NULL) {
    cout << " " << temp->data;
    traversePreOrder(temp->left);
    traversePreOrder(temp->right);
  }
}

// Traverse Inorder
void traverseInOrder(struct node *temp) {
  if (temp != NULL) {
    traverseInOrder(temp->left);
    cout << " " << temp->data;
    traverseInOrder(temp->right);
  }
}

// Traverse Postorder
void traversePostOrder(struct node *temp) {
  if (temp != NULL) {
    traversePostOrder(temp->left);
    traversePostOrder(temp->right);
    cout << " " << temp->data;
  }
}

```


## Output:
<img width="722" height="439" alt="image" src="https://github.com/user-attachments/assets/75c8e365-147f-4f5e-87de-3696800f9470" />



## Result:
The functions successfully perform all three tree traversals and display the nodes in the following orders:

