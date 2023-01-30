## Question 3052


```python 3
arr = [] #리스트
for i in range(10):
    a = int(input())
    if a%42 not in arr: #if 문으로 추출
        arr.append(a % 42) # append 로 추출값 저장
print(len(arr))

```


### Example:
<img width="1189" alt="스크린샷 2023-01-31 오전 4 41 21" src="https://user-images.githubusercontent.com/107760647/215578908-b87773ad-6d31-4c83-b6f6-cebf46edb72b.png">


Reference:
https://www.acmicpc.net/problem/3052
