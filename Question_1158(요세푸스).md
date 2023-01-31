## Question 1158 (요세푸스)


```python 3
N,K = map(int,input().split())
arr = [i for i in range(1,N+1)]    # 맨 처음에 원에 앉아있는 사람들

answer = []   # 제거된 사람들을 넣을 배열
num = 0  # 제거될 사람의 인덱스 번호

for t in range(N):
    num += K-1  
    if num >= len(arr):   # 한바퀴를 돌고 그다음으로 돌아올때를 대비해 값을 나머지로 바꿈  
        num = num%len(arr)
 
    answer.append(str(arr.pop(num))) # pop = list 에서 값 지움
print("<",", ".join(answer)[:],">", sep='')
```


### Example:
<img width="1202" alt="스크린샷 2023-02-01 오전 5 47 55" src="https://user-images.githubusercontent.com/107760647/215879381-3499dc3f-35e6-466f-8011-2d9ad00bc039.png">


Reference:
https://www.acmicpc.net/problem/1158
