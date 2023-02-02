## Question 2908


```python 3
A, B = input().split()

if int(A[::-1]) > int(B[::-1]): # ::-1 = 역순
    print(A[::-1])
else:
    print(B[::-1])

```


### Example:
<img width="1247" alt="스크린샷 2023-02-03 오전 5 01 29" src="https://user-images.githubusercontent.com/107760647/216437197-597923b6-2af3-4636-adcb-de832fd2072f.png">


Reference:
https://www.acmicpc.net/problem/2908
