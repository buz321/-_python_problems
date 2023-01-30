## Question 1546


```python 3
A = int(input())
score = list(map(int,input().split()))

avg = 0
for i in range(A):
    avg += score[i] / max(score) * 100 # 왼쪽 변수에 오른쪽 값을 더하고 그 결과를 왼쪽 변수에 할당, could use sum() as well
print(avg / A)

```


### Example:
<img width="1261" alt="스크린샷 2023-01-31 오전 4 57 46" src="https://user-images.githubusercontent.com/107760647/215582134-8eda8702-0159-4120-bfdc-096d63a3973b.png">


Reference:
https://www.acmicpc.net/problem/1546
