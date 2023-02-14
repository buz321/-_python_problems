## Question 1427


```python 3
N = int(input())
 
nayeol = [] # 나열 리스트 생성
for i in str(N): # 포문을 활용하여
    nayeol.append(int(i)) # 리스트에 숫자 저장
 
nayeol.sort(reverse=True) # sort()로 오름차순 정렬
 
for i in nayeol: #포문을 활용하여
    print(i, end='') # 값 출력, end=''를 주어 한줄에 출력이되도록 한다.

```


### Example:
<img width="1176" alt="스크린샷 2023-02-15 오전 5 25 14" src="https://user-images.githubusercontent.com/107760647/218853954-a513985b-9fa7-432b-a7de-123d6b46bcc2.png">


Reference:
https://www.acmicpc.net/problem/1427
