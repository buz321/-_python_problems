## Question 10807


```python 3
A = int(input())
B = map(int,input().split())
v = int(input())

cnt = 0
for i in B:
    if i == v:
        cnt += 1
print(cnt)

```


### Example:
<img width="1213" alt="스크린샷 2023-01-23 오전 4 46 46" src="https://user-images.githubusercontent.com/107760647/213936967-9cf38837-0e54-4ac5-abe6-0681f8aafbd9.png">


Reference:
https://www.acmicpc.net/problem/10807
