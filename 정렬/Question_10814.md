## Question 10814


```python 3
import sys
N=int(sys.stdin.readline()) #input() 대신

li=[] # 리스트 설정

for i in range (N): 
  a,b = map(str,sys.stdin.readline().split()) 
  li.append([int(a), b]) # a= 나이 정수로 받음

li.sort(key=lambda x:x[0]) # 리스트 0 번째 = 나이 올림차순 설정

for i in li:
  print(*i, sep=" ") # i는 리스트 형식 없애주는 역할

```


### Example:
<img width="1239" alt="스크린샷 2023-02-16 오전 5 32 37" src="https://user-images.githubusercontent.com/107760647/219147795-5bbb566e-2db2-4d53-b946-cc85f942a3a8.png">


Reference:
https://www.acmicpc.net/problem/10814
