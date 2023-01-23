## Question 10871


```python 3
N, X = map(int, input().split())
A = list(map(int, input().split()))
for i in range(N):
    if A[i] < X:
        print(A[i], end=" ")

```


### Example:
<img width="1194" alt="스크린샷 2023-01-24 오전 7 50 53" src="https://user-images.githubusercontent.com/107760647/214169879-3187b270-7b62-4f50-9e0a-74babfa468e6.png">


Reference:
https://www.acmicpc.net/problem/10871
