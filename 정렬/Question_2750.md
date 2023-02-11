## Question 2750


```python 3
N = int(input())
 
nayeol = [] # 나열 리스트 생성
for i in range(N): # 포문을 활용하여
    nayeol.append(int(input())) # 리스트에 숫자 저장
 
nayeol.sort() # sort()로 오름차순 정렬
 
for i in nayeol: #포문을 활용하여
    print(i) # 값 출력

```


### Example:
<img width="1198" alt="스크린샷 2023-02-11 오후 10 54 40" src="https://user-images.githubusercontent.com/107760647/218261683-104d76c0-1e27-4112-aee5-337901d518fa.png">


Reference:
https://www.acmicpc.net/problem/2750
