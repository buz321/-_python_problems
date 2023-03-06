## Question 1269


```python 3
A,  B = map(int, input().split())
A_li = set(map(int, input().split()))
B_li = set(map(int, input().split()))
print(len(A_li - B_li) + len(B_li - A_li))

```


### Example:
<img width="1275" alt="스크린샷 2023-03-07 오전 4 57 28" src="https://user-images.githubusercontent.com/107760647/223217048-337366c6-7c32-41f0-b7a1-c0fc7d86bf86.png">



Reference:
https://www.acmicpc.net/problem/1269
