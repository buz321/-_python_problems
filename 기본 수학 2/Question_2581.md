## Question 2581


```python 3
M = int(input())
N = int(input())
sosu = []

for i in range(M, N + 1):  # 처음 숫자부터 (M) ~ (N)
    cnt = 0 #  카운트
    if i == 1 : # 만약 숫자가 1이면 소수가 아니므로 패스
          continue

    for j in range(2, i): # 2부터 n-1까지 이중 포문
        if i % j == 0: # 예를 들어 i 9를 2~9 부터 숫자중 나누어 떨어지는 숫자 3,9
            cnt += 1 # 2부터 n-1까지 나눈 몫이 0이면 카운트가 증가
            break
    if cnt == 0: # error 가 0개이면 소수, 소수리스트에 추가
        sosu.append(i) #참고: append = list에 추가

if len(sosu) > 0: 
    print(sum(sosu)) # 가능한 소수의 모두를 더한 값
    print(min(sosu)) # 소수 최솟값
else:
    print(-1) 

```


### Example:
<img width="1198" alt="스크린샷 2023-02-10 오전 5 34 25" src="https://user-images.githubusercontent.com/107760647/217930747-f2f261ca-2f58-4be0-abfb-f78f9298def1.png">


Reference:
https://www.acmicpc.net/problem/2581
