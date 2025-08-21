# Ex19 B+ Tree
## DATE: 25/05/2025
## AIM:
To write a C function to traverse the elements in a B+ Tree.

## Algorithm
1. Start
2. Iterate through each element in the node's data array.
3. If the node is not a leaf, recursively call traverse on the current child pointer.
4. Print the current data element.
5. After the loop, if the node is not a leaf, traverse the last child pointer.
6. Return after completing the traversal.
7. End  

## Program:
```
/*
Program to traverse the elements in a B+ Tree.
Developed by: MOHAMED RASHITH S
RegisterNumber: 212223243003 
*/
struct B_TreeNode
{
int*data;
structB_TreeNode**child_ptr; int leaf;
int n;
};
struct B_TreeNode*root =NULL, *np=NULL, *x =NULL;*/

voidtraverse(struct B_TreeNode*p)
{
int i;
for(i=0;i<p->n;i++)
{
if(p->leaf==0)
{
traverse(p->child_ptr[i]);
}
printf("%d",p->data[i]);
}
if(p->leaf==0)
{
traverse(p->child_ptr[i]);
}
}
```

## Output:

![image](https://github.com/user-attachments/assets/c0d92237-8a29-42c0-98d0-28cb84f69e10)


## Result:
Thus, the function to traverse the elements in a B+ Tree is implemented successfully.
