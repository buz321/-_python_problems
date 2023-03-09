## Question 2740


```python 3
N, M = map(int, input().split())
A = []
for _ in range(N):
    A.append(list(map(int, input().split())))

M, K = map(int, input().split())
B = []
for _ in range(M):
    B.append(list(map(int, input().split())))


#행렬 곱셈
C = [[0 for _ in range(K)] for _ in range(N)]

for n in range(N):
    for k in range(K):
        for m in range(M):
            C[n][k] += A[n][m] * B[m][k] # N*K 곱하기 M*K = N*K 구현

#출력문
for i in C:
    for j in i:
        print(j, end = ' ')
    print()

```


### Example:
<img width="1245" alt="스크린샷 2023-03-10 오전 3 35 19" src="https://user-images.githubusercontent.com/107760647/224122620-50c28e98-60ca-43e9-9c75-028f9cee5ca9.png">


Reference:
https://www.acmicpc.net/problem/2740
