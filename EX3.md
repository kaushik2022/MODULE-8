# Ex.No:3
# Ex.Name :  Write a C++ Function to perform Inorder traversal of the below given tree
## Date: 25/09/2025
## Aim:
To write a C++ function to perform inorder traversal on a binary tree and print the node values as a single line of space-separated values.
## Algorithm:
```
Start the function.

If the root is NULL, return.

Recursively traverse the left subtree.

Print the root node's data.

Recursively traverse the right subtree.

End the function.
```
## Program:
```cpp
// Traverse Inorder
void traverseInOrder(struct node *temp) {
  if (temp != NULL) {
    traverseInOrder(temp->left);
    cout << " " << temp->data;
    traverseInOrder(temp->right);
  }
}

```


## Output:
<img width="741" height="532" alt="image" src="https://github.com/user-attachments/assets/579bdcab-b931-4aa5-9d4b-66a1908b1b5d" />



## Result:
The function successfully performs inorder traversal of the given binary tree and prints the node values in the order:
Left Subtree → Root → Right Subtree


