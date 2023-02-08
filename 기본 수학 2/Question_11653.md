## Question 11653


```python 3
n = int(input())
so = 2 # 소인수분해를 2부터 시작
while n != 1: # 1은 제외
    if n%so == 0: # n이 so 로 나누어 떨어지면 
        n = n // so
        print(so) # so 를 출력
    else:
        so+=1 # 아닌 경우엔 so 에 1을 계속 더해나감

```


### Example:
<img width="1173" alt="스크린샷 2023-02-09 오전 5 29 25" src="https://user-images.githubusercontent.com/107760647/217643942-c489b24c-638d-45fc-8d1f-7ccaf7e6449d.png">


Reference:
https://www.acmicpc.net/problem/11653
