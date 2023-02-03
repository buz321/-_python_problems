## Question 2941


```python 3
croatia = ['c=', 'c-', 'dz=', 'd-', 'lj', 'nj', 's=', 'z=']
word = input()

for i in croatia :
    word = word.replace(i, '*')  # input 변수와 동일한 이름의 변수
print(len(word)) # 갯수 출력

```


### Example:
<img width="1195" alt="스크린샷 2023-02-04 오전 4 12 54" src="https://user-images.githubusercontent.com/107760647/216687563-5feaeae8-d79e-47f0-8c3b-95e3633e9416.png">


Reference:
https://www.acmicpc.net/problem/2941
