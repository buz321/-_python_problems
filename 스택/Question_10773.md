## Question 10773


```python 3
n = int(input())
li = []
for i in range(n): # 포문 설정
    num = int(input()) 
    if num == 0:
        li.pop() # 만약 입력값이 0 이면 이전값 삭제
    else:
        li.append(num) # 다른 값들은 추가 
print(sum(li)) # 삭제된 값을 제외하고 모든 값의 합 출력

```


### Example:
<img width="1215" alt="스크린샷 2023-03-09 오전 5 12 01" src="https://user-images.githubusercontent.com/107760647/223838148-227be11f-8729-4ff0-ab86-fcd0e47a188e.png">


Reference:
https://www.acmicpc.net/problem/10773
