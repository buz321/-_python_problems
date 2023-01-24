## Question 5597


```python 3
# 1부터 30까지의 리스트를 생성 
num = [i for i in range(1, 31)]

# 입력받은 숫자를 리스트에서 제거
for _ in range(28):
    data = int(input())
    num.remove(data)
print(min(num))
print(max(num))

```


### Example:
<img width="1201" alt="스크린샷 2023-01-25 오전 8 18 47" src="https://user-images.githubusercontent.com/107760647/214442614-04a2f961-3649-4db2-a66f-045552ad728f.png">


Reference:
https://www.acmicpc.net/problem/5597
