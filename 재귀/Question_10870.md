## Question 10870


1번째 방법 = for loop
```python 3
n = int(input())

fibonacci = [0,1]
for i in range (2,n+1):
    fib = fibonacci[i-1] + fibonacci[i-2]
    fibonacci.append(fib)
print(fibonacci[n])

```

2번째 방법 = 재귀함수
```python 3
def fibo(n):
    if n < 2:
        return n
    else:
        return fibo(n-1) + fibo(n-2)
print(fibo(int(input())))
```


### Example:
<img width="1182" alt="스크린샷 2023-02-16 오전 5 54 03" src="https://user-images.githubusercontent.com/107760647/219156330-bdc8b1e6-1b6e-4b8f-89c2-ee4f09813ce2.png">


Reference:
https://www.acmicpc.net/problem/10870
