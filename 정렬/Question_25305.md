## Question 25305


```python 3
N,k = map(int,input().split())
score = list(map(int,input().split()))
score.sort(reverse=True) # 내림차순으로 정리
print(score[k-1]) # k 리스트 에서 2번째 값 출력

```


### Example:
<img width="1257" alt="스크린샷 2023-02-14 오전 5 11 20" src="https://user-images.githubusercontent.com/107760647/218564450-30f03ed0-ab8d-4a2e-aeb4-9a364ff4e334.png">


Reference:
https://www.acmicpc.net/problem/25305
