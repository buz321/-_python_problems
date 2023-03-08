## Question 2164


```python 3
n = int(input())
s = 2 # 식 계산을 위한 값 설정

while True: # while 문 설정
    if (n == 1 or n == 2): 
        print(n) # n이 1 과 2일때는 규칙이 없기때문에 따로 설정
        break
    s *= 2
    if (s >= n): # 규칙 설정
        print((n- (s // 2)) * 2)
        break

```


### Example:
<img width="1207" alt="스크린샷 2023-03-09 오전 4 51 24" src="https://user-images.githubusercontent.com/107760647/223830297-febd8374-4aed-4ea9-aa99-d52f3af13fcf.png">


Reference:
https://www.acmicpc.net/problem/2164
