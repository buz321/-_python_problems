## Question 2839


```python 3
N=int(input())

bag = 0
while N >= 0:
    if N % 5 == 0: # 5의 배수로 떨어지면
        bag += (N//5) # 5로 나눈 몫을 계속 더함
        print(bag)
        break
    N -= 3 # 5의 배수가 될때까지 -3을 함
    bag += 1
else:
    print(-1) # 두 수로 안떨어지면 -1 출력

```


### Example:
<img width="1211" alt="스크린샷 2023-02-08 오전 5 23 54" src="https://user-images.githubusercontent.com/107760647/217356792-d1acb133-6782-430c-8820-44ece501aaaf.png">


Reference:
https://www.acmicpc.net/problem/2839
