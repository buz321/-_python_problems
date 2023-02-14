## Question 11651


```python 3
import sys

N = int(input())

nayeol = []
for i in range(N):
    x, y = map(int, sys.stdin.readline().split())
    nayeol.append([y,x]) # 문제상 y좌표가 증가하게 짜야하므로 y를 앞으로 빼서 

s_nayeol = sorted(nayeol) # 디폴트 올림차순!

for y,x  in s_nayeol:
    print(x, y) # 값을 출력할때는 원상태로 출력

```


### Example:
<img width="1202" alt="스크린샷 2023-02-15 오전 5 56 49" src="https://user-images.githubusercontent.com/107760647/218861330-fc342824-142f-47ec-bdee-361517b07506.png">


Reference:
https://www.acmicpc.net/problem/11651
