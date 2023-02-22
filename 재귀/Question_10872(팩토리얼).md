## Question 10872 (팩토리얼)



```python 3
N = int(input())

fac = 1 # 0!은 1로 나오게 설정 (수학원리) 
if N > 0:
    for i in range(1, N+1):
        fac *= i # i값을 다 곱해서 저장
print(fac) # 값 출력

```



### Example:
<img width="1178" alt="스크린샷 2023-02-17 오전 3 51 20" src="https://user-images.githubusercontent.com/107760647/219459998-55a53270-ed37-4ffd-b5de-c24aeb7f8929.png">


Reference:
https://www.acmicpc.net/problem/10872
