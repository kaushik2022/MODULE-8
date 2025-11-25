# Ex.No:2
# Ex.Name :  Write a C++ Function to perform Preorder traversal of the below given tree
## Date: 25/09/2025
## Aim:
To write a C++ function to perform preorder traversal on a binary tree and print the node values as a single line of space-separated values.
## Algorithm:
```
1.Start the function.

2.If the root is NULL, return.

3.Print the root node's data.

4.Recursively traverse the left subtree.

5.Recursively traverse the right subtree.

6.End the function.
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

```


## Output:
<img width="675" height="526" alt="image" src="https://github.com/user-attachments/assets/55b3525d-f1f0-42d3-9860-c0bb704da14f" />



## Result:
The function successfully performs preorder traversal of the given binary tree and prints the node values in the order:
Root → Left Subtree → Right Subtree

