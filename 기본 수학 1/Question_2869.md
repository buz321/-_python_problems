## Question 2869


```python 3
a,b,v = map(int,input().split())
k = (v-b)/(a-b) # ak + (-b)(k-1) = v, a는 올라가는 수 +, b는 내려가는 수 -
print(int(k) if k == int(k) else int(k)+1) # 분수인경우 +1 (올림) = 층을 나타내야 함으로

```


### Example:
<img width="1211" alt="스크린샷 2023-02-06 오전 8 17 44" src="https://user-images.githubusercontent.com/107760647/216851607-00ae20b5-cb9b-452b-8af3-e1505a8e7ffc.png">


Reference:
https://www.acmicpc.net/problem/2869
