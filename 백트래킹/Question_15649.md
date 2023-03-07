## Question 15649


```python 3
n, m = map(int, input().split())

s = []
def f(): # 재귀 함수
  if len(s) == m:
    print(' '.join(map(str, s)))
    return

  for i in range(1, n + 1):
    if i in s: # pruning 작업: 이미 선택한 숫자를 다시 선택하려 하면 배제하는 방식
      continue
    s.append(i)
    f()
    s.pop() # 다시 s에서 빼내는 작업
            # 정상적으로 이전으로 돌아가기 위해
            # 그렇게 선택을 반복했을 때, 그 선택한 경우의 수가 m이 되면 모두 고른 것이 되므로 해답이 된다.

f()

```
<img width="809" alt="스크린샷 2023-03-08 오전 4 17 05" src="https://user-images.githubusercontent.com/107760647/223527593-21e5d7f8-5e6e-4c78-b9ec-763c1ab36c5a.png">

* 백트래킹: 불필요한 경우를 배제하며 원하는 해답에 도달할 때까지 탐색하는 전략이다
* 위 그림과 같이, DFS를 기반으로 두고 있기 때문에 스택(Stack)을 이용해 퇴각을 하며 다음 탐색을 진행하기 때문에 백트래킹(또는 퇴각검색)이라 불린다.


### Example:
<img width="1178" alt="스크린샷 2023-03-08 오전 4 15 15" src="https://user-images.githubusercontent.com/107760647/223527234-8b609c86-9b3b-456c-b2b6-969f5644df73.png">


Reference:
https://www.acmicpc.net/problem/15649
