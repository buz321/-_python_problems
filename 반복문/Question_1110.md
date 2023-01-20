## Question 1110


```python 3
N = int(input())  #입력받은 값을 int로 바꿈
num = N           #변하는 값
count = 0         #몇 번 사이클인지
 
while True:
    a = num//10
    b = num %10
    c = (a+b)%10
    num = (b*10) + c
    count += 1
    if(num == N):
        break
 
print(count)
```


### Example:
<img width="1204" alt="스크린샷 2023-01-21 오전 7 21 26" src="https://user-images.githubusercontent.com/107760647/213815554-2b94f299-5655-494e-88d3-928c2ab4f1cb.png">


Reference:
https://www.acmicpc.net/problem/1110
