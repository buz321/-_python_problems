## Question 2775


```python 3
T=int(input())

for i in range(T):
    k=int(input())
    n=int(input())
    base=[j for j in range(1,n+1)]
    for l in range(k):
        for m in range(1,n):
            base[m]+=base[m-1]
    print(base[n-1])

```


### Example:
<img width="1210" alt="스크린샷 2023-02-05 오전 2 22 33" src="https://user-images.githubusercontent.com/107760647/216780899-f80dfb63-4e92-4416-8e75-e585d0cccef8.png">


Reference:
https://www.acmicpc.net/problem/2775
