## Question 10809


```python 3
S = input()
alph ='abcdefghijklmnopqrstuvwxyz'

for i in alph:
    if i in S:
        print(S.index(i), end= ' ')
    else:
        print( -1, end =' ')

```


### Example:
<img width="1257" alt="스크린샷 2023-02-03 오전 3 31 32" src="https://user-images.githubusercontent.com/107760647/216417187-6d4740f2-5966-4970-8a1e-e66f376fa0cd.png">


Reference:
https://www.acmicpc.net/problem/10809
