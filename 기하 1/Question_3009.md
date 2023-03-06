## Question 3009


```python 3
# x,y 값 리스트로 표현
x_li = []
y_li = []
for i in range(3):
        x, y = map(int, input().split())
        x_li.append(x) # x,y 값을 리스트에 저장
        y_li.append(y)
for i in range(3):
        if x_li.count(x_li[i]) == 1:
                x = x_li[i]
        if y_li.count(y_li[i]) == 1:
                y = y_li[i]
print(x, y) #요소의 개수를 세어서 개수가 하나인것을 출력

```


### Example:
<img width="1185" alt="스크린샷 2023-03-07 오전 5 10 59" src="https://user-images.githubusercontent.com/107760647/223219764-48e12ab0-ce0c-4cea-9cc3-5050f1f017c4.png">



Reference:
https://www.acmicpc.net/problem/3009
