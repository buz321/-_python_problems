## Question 11725


```python 3
import sys
 
N = int(sys.stdin.readline().strip())
tree = {}
 
for n in range(N):
    root, left, right = sys.stdin.readline().strip().split()
    tree[root] = [left, right]
 
 
def preorder(root):
    if root != '.':
        print(root, end='')  # root
        preorder(tree[root][0])  # left
        preorder(tree[root][1])  # right
 
 
def inorder(root):
    if root != '.':
        inorder(tree[root][0])  # left
        print(root, end='')  # root
        inorder(tree[root][1])  # right
 
 
def postorder(root):
    if root != '.':
        postorder(tree[root][0])  # left
        postorder(tree[root][1])  # right
        print(root, end='')  # root
 
 
preorder('A')
print()
inorder('A')
print()
postorder('A')

```


### Example:
<img width="1203" alt="스크린샷 2023-03-14 오전 5 24 26" src="https://user-images.githubusercontent.com/107760647/224823996-101e588c-6166-4758-bcc1-b2548cae0931.png">


Reference:
https://www.acmicpc.net/problem/1991
