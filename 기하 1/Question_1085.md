## Question 1085


```python 3
x, y, w, h = map(int, input().split())
print(min(x, y, w-x, h-y)) #거리의 최솟값

```


### Example:
<img width="1176" alt="스크린샷 2023-03-07 오전 4 58 14" src="https://user-images.githubusercontent.com/107760647/223217197-d7ecd38e-12f6-477a-9eb2-9f2ceb82bd35.png">



Reference:
https://www.acmicpc.net/problem/1085
