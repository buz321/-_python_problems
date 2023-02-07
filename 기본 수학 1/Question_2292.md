## Question 2292


```python 3
N=int(input())
comb= 1 # 벌집 갯수
cnt = 1
while N > comb:
    comb += 6 * cnt # 벌집 지날수록 6의 배수로 증가
    cnt += 1 # 지날수록 1을 더 카운트
print(cnt) # 벌집 거치는 개수를 출력

```


### Example:
<img width="1235" alt="스크린샷 2023-02-08 오전 5 10 18" src="https://user-images.githubusercontent.com/107760647/217354163-6249b496-d1ec-48ed-a5e0-9b4170d41041.png">


Reference:
https://www.acmicpc.net/problem/2292
