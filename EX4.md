# Ex.No:4
# Ex.Name :  Write a C++ Function to perform Postorder traversal of the below given tree
## Date: 25/09/2025
## Aim:
To write a C++ function to perform postorder traversal on a binary tree and print the node values as a single line of space-separated values.
## Algorithm:
```
Start the function.

If the root is NULL, return.

Recursively traverse the left subtree.

Recursively traverse the right subtree.

Print the root node’s data.

End the function
```
## Program:
```cpp
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
<img width="726" height="397" alt="image" src="https://github.com/user-attachments/assets/08252254-f3d2-4e8d-b8e5-ac585e547162" />



## Result:
The function successfully performs postorder traversal of the given binary tree and prints the node values in the order:
Left Subtree → Right Subtree → Root

