## Question 2587


```python 3
nayeol = [] # 나열 리스트 생성
for i in range(5): # 포문을 활용하여
    nayeol.append(int(input())) # 리스트에 숫자 저장
nayeol.sort() # 리스트 정리
print(int(sum(nayeol)/5)) # 전체 합계에서 전체 개수로 나눔 (개수가 5개로 고정이니 5로 나눔)
print(nayeol[2]) # 중간에 있는 값 (리스트 0,1,2,3,4)

```


### Example:
<img width="1206" alt="스크린샷 2023-02-13 오전 6 49 48" src="https://user-images.githubusercontent.com/107760647/218339268-d30d5f0f-82f8-47b8-b4a7-9382cedb2830.png">


Reference:
https://www.acmicpc.net/problem/2587
