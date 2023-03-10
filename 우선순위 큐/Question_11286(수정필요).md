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
            print(heapq.heappop(heap)[1])
        else:
            print(0)
    else:
        heapq.heappush(heap,(abs(x),x))

```


### Example:
<img width="1226" alt="스크린샷 2023-03-11 오전 4 56 35" src="https://user-images.githubusercontent.com/107760647/224415310-1d245279-451f-42e0-b1fc-2b705d39abb8.png">


Reference:
https://www.acmicpc.net/problem/11286
