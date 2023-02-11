## Question 1929


```python 3
M,N=map(int,input().split(' '))

for num in range(M,N+1):
    if num==1: # 만약 숫자가 1이면 소수가 아님으로 패스
        continue
    for i in range(2,int(num**0.5)+1): # 제곱근까지만 검사
        if num%i==0: # 예를 들어 어차피 소인수분해를 하게되면 모든 수는 대칭적으로 뽑아지기 때문에, 제곱근까지만 검사
            break   
    else:
        print(num) 

```


### Example:
<img width="1188" alt="스크린샷 2023-02-11 오후 10 52 40" src="https://user-images.githubusercontent.com/107760647/218261616-073504b0-a9bd-4915-aaba-33730bb8823a.png">


Reference:
https://www.acmicpc.net/problem/1929
