## Question 1978


```python 3
n = int(input())
numbers = map(int, input().split(' ')) 
sosu = 0
for num in numbers:
    cnt = 0 # 에러 카운트
    if num == 1 : # 만약 숫자가 1이면 소수가 아님으로 패스
          continue
    
    for i in range(2, num + 1):  # 2부터 n-1까지 이중 포문
        if num % i == 0: # 예를 들어 i 9를 2~9 부터 숫자중 나누어 떨어지는 숫자 3,9
            cnt += 1  # 2부터 n-1까지 나눈 몫이 0이면 error가 증가
                
    if cnt == 1: # error 가 1개이면 소수, 2개이면 나누어 떨어지는 숫자가 2개 이므로 카운트가 안됨
        sosu += 1  # error가 없으면 소수.
print(sosu)

```


### Example:
<img width="1188" alt="스크린샷 2023-02-09 오전 5 53 24" src="https://user-images.githubusercontent.com/107760647/217648554-0e71d4a6-97d9-477a-8085-d8133a68466e.png">


Reference:
https://www.acmicpc.net/problem/1978
