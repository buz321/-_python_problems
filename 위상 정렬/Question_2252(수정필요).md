## Question 2252


```python 3
import sys
from collections import deque

n, m = map(int, sys.stdin.readline().split())

graph = [[] for _ in range(n+1)]
inDegree = [0 for _ in range(n+1)]
queue = deque() # 입력값을 각각의 개체로 분류 
answer = []

for i in range(m):
    a, b = map(int, sys.stdin.readline().rstrip().split())
    graph[a].append(b)
    inDegree[b] += 1

for i in range(1, n+1):
    if inDegree[i] == 0:
        queue.append(i)

while queue:
    tmp = queue.popleft()
    answer.append(tmp)
    for i in graph[tmp]:
        inDegree[i] -= 1
        if inDegree[i] == 0:
            queue.append(i)

print(*answer)

```


### Example:
<img width="1177" alt="스크린샷 2023-03-16 오전 5 46 24" src="https://user-images.githubusercontent.com/107760647/225438164-754e6649-db92-4aee-ad46-f8bcfc5a0163.png">


Reference:
https://www.acmicpc.net/problem/2252
