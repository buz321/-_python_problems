## Question 2675


```python 3
S = int(input())

for _ in range(S):
    R, P = input().split()
    for i in P:
        print(i*int(R), end='')  # end='' 옆으로 붙임
    print() # 1이상의 값 줄 넘겨넣기

```


### Example:
<img width="1174" alt="스크린샷 2023-02-03 오전 3 39 44" src="https://user-images.githubusercontent.com/107760647/216419495-2f08e949-07ad-4c67-bcc4-58be0458eb1a.png">


Reference:
https://www.acmicpc.net/problem/2675
