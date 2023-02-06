## Question 1712


```python 3
A, B, C = map(int, input().split())

if B>=C:
    print(-1) 
else:
    print(int(A/(C-B)+1)) # 올림 값

```


### Example:
<img width="1214" alt="스크린샷 2023-02-07 오전 5 38 13" src="https://user-images.githubusercontent.com/107760647/217079908-3bf13ca5-0835-43d2-9f0c-ecb30e6666b3.png">


Reference:
https://www.acmicpc.net/problem/1712
