## Question 1181


```python 3
n = int(input())

word = []
for i in range(n):
    word.append(input()) # 단어 리스트에 추가

set_word = list(set(word)) # set을 이용해 중복 제거

sort_word = []
for i in set_word:
    sort_word.append((len(i), i)) #또 다른 리스트를 추가해, 단어의 길이를 추가

result = sorted(sort_word) # 올림차순 정리

for len_word, word in result:
    print(word)
```


### Example:
<img width="1248" alt="스크린샷 2023-02-16 오전 5 25 54" src="https://user-images.githubusercontent.com/107760647/219146146-8c68384e-f09e-4b15-8828-2880d968145e.png">


Reference:
https://www.acmicpc.net/problem/1181
