## Question 25304


```python 3
A = int(input()) # total price
B = int(input()) # total number of products

sum = 0

for i in range(1,B+1):
    C,D= map(int,input().split()) # each product's price and amount
    sum += C*D
 
if A==sum: print("Yes")
else: print("No")
```


### Example:
<img width="1359" alt="스크린샷 2023-01-20 오전 6 11 59" src="https://user-images.githubusercontent.com/107760647/213560380-02d29a87-b722-4d8c-a666-af258d4f5ff7.png">


Reference:
https://www.acmicpc.net/problem/25304
