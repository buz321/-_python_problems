## Question 2751


```python 3
import sys

N = int(input())
nayeol = []
for i in range(N):
    nayeol.append(int(sys.stdin.readline())) #시간제한 때문에 input() 사용 불가능 = 느려서
# input() 내장 함수는 sys.stdin.readline()과 비교해서 prompt message를 출력하고, 개행 문자를 삭제한 값을 리턴하기 때문에 느리다.

nayeol.sort()

for i in nayeol:
    print(i)

```

### Example:
<img width="1225" alt="스크린샷 2023-02-14 오전 5 59 33" src="https://user-images.githubusercontent.com/107760647/218573282-9df36d42-5fc2-4bd3-b282-997cac871640.png">


Reference:
https://www.acmicpc.net/problem/2751
