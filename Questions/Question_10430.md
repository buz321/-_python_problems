## Question 10430


```python 3
A,B,C = map(int,input().split())
print((A+B)%C, ((A&C)+(B%C))%C, (A*B)%C, ((A&C)*(B%C))%C, sep='\n')
```
<img width="957" alt="스크린샷 2023-01-17 오전 5 50 12" src="https://user-images.githubusercontent.com/107760647/212763643-7e70c28e-791d-4a03-b306-28f0a9d673ea.png">


### Example:
<img width="1181" alt="스크린샷 2023-01-17 오전 5 44 15" src="https://user-images.githubusercontent.com/107760647/212762791-c6e44bda-0d3a-4547-b761-aade506c3bbd.png">


Reference:
https://www.acmicpc.net/problem/10430
