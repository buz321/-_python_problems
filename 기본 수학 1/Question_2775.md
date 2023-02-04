## Question 2775


```python 3
T=int(input()) # Test Case

for i in range(T):
    k=int(input()) #층
    n=int(input()) #호수
    base=[j for j in range(1,n+1)] # 0층 리스트
    for l in range(k):  # 층 수 만큼 반복
        for m in range(1,n): # 1 ~ n-1까지 (인덱스로 사용)
            base[m]+=base[m-1] # 층별 각 호실의 사람 수를 변경
    print(base[n-1])

```


### Example:
<img width="1210" alt="스크린샷 2023-02-05 오전 2 22 33" src="https://user-images.githubusercontent.com/107760647/216780899-f80dfb63-4e92-4416-8e75-e585d0cccef8.png">


Reference:
https://www.acmicpc.net/problem/2775
