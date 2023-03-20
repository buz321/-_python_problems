## Question 4948 베르트랑 공준


```python 3
import math

m = 123456 # m의 범위의 최댓값

array1 = [True for _ in range(2 * m + 1)] #소수 판별을 위한 리스트설정(True면 소수)
array1[0], array1[1] = False, False #0,1은 소수가 아니기에 False로 설정 = 리스트로 표기

# 에라토스테네스의 체 공식
for i in range(2, int(math.sqrt(2 * m) + 1)): #2부터 int(math.sqrt(2 * 123456) 까지 돈다.
    if array1[i]: #만약 array1[i]가 True(소수)라면
        j = 2 #i에 곱해줄 j값을 2부터 설정
        while i * j <= 2 * m: #i * j 가 2* 123456 보다 작거나 같다면
            array1[i * j] = False #해당 i*j의 값은 소수가 아니므로 False로 설정
            j += 1 #j를 1씩 증가

while True:
    n = int(input())
    if n == 0: #0이면 반복문 탈출
        break

    count = 0
    # 개수 출력
    for i in range(n+1, 2 * n + 1): #n+1(n보다 커야하기 때문) 부터 2 * n + 1 까지 설정
        if array1[i]:  #만약 해당 i가 True(소수) 라면
            count += 1 #count값에다 +1
    print(count)  #count 값 출력
```

* 네이버 수학 백과 참고: https://terms.naver.com/entry.naver?docId=5669298&cid=60207&categoryId=60207

### Example:
<img width="1208" alt="스크린샷 2023-03-21 오전 5 05 37" src="https://user-images.githubusercontent.com/107760647/226453450-c5c4c3ef-2fb4-4121-a2fe-ff5bc4ca3230.png">


Reference:
https://www.acmicpc.net/problem/4948
