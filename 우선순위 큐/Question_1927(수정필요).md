## Question 1927


```python 3
import sys
import heapq

n = int(input())
heap = []

#Max Heap
for _ in range(n):
    num = int(sys.stdin.readline())
    if num != 0:
        heapq.heappush(heap, num)
    else:
        try:
            print(heapq.heappop(heap))
        except:
            print(0)

```


### Example:
<img width="1233" alt="스크린샷 2023-03-12 오전 6 34 26" src="https://user-images.githubusercontent.com/107760647/224512482-0611d875-282c-4f8e-bf52-f117201543ac.png">


Reference:
https://www.acmicpc.net/problem/1927
