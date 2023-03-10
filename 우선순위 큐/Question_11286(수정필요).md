## Question 11286


```python 3
import sys
import heapq

n = int(input())
heap = []
for i in range(n):
    x = int(sys.stdin.readline())
    if x == 0:
        if heap:
            print(heapq.heappop(heap)[1]) # pop을 해줄 때는 heapq.heappop(heap)[1]로 해서 뒤에 있는 원래 값을 출력
        else:
            print(0)
    else:
        heapq.heappush(heap,(abs(x),x)) # heap에 push를 할 때 (절댓값, 원래값)을 같이 넣어줘서 만약 절댓값이 같으면 원래 값이 음수인 것이 먼저 출력

```
* abs = 절댓값 연산

### Example:
<img width="1226" alt="스크린샷 2023-03-11 오전 4 56 35" src="https://user-images.githubusercontent.com/107760647/224415310-1d245279-451f-42e0-b1fc-2b705d39abb8.png">


Reference:
https://www.acmicpc.net/problem/11286
