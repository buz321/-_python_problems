## Question 2252 (위상정렬)


```python 3
import sys
from collections import deque
input = sys.stdin.readline

N, M = map(int, input().split())
graph = [[] for _ in range(N+1)]
inDegree = [0]*(N+1) # 진입차수 

for _ in range(M):
    A, B = map(int, input().split())
    graph[A].append(B)
    inDegree[B] += 1

q = deque() # 입력값을 각각의 개체로 분류

for s in range(1, N+1):
    if inDegree[s] == 0: # 최초 진입 차수를 0으로 설정
        q.append(s) # 0을 큐에 집어 넣음

ans = []

while q: # while 문 
    s = q.popleft()
    ans.append(s)
    
    for adj_s in graph[s]:
        inDegree[adj_s] -= 1
        if inDegree[adj_s] == 0:
            q.append(adj_s)

print(*ans, sep=" ")

```
* 전형적인 위상 정렬 문제
* 조금 더 파고 들 필요 있
* 위상 정렬 알고리즘 참고: https://terms.naver.com/entry.naver?docId=3579618&cid=59086&categoryId=59093

### Example:
<img width="1177" alt="스크린샷 2023-03-16 오전 5 46 24" src="https://user-images.githubusercontent.com/107760647/225438164-754e6649-db92-4aee-ad46-f8bcfc5a0163.png">




Reference:
https://www.acmicpc.net/problem/2252
