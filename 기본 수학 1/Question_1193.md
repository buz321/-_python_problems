## Question 1193


```python 3
X = int(input())

line = 0  # 몇번째 라인?
max_num = 0  # 변수 라인에서 가장 큰 숫자
while X > max_num: 
    line += 1  
    max_num += line # e.g. 1,3,6,10 .....  

diff = max_num - X # 전체 합계 - 입력 값 = 해당 위치의 숫자를 구하기 위해
if line % 2 == 0:  # 라인이 짝수번째 일 때
    boonja = line - diff  #분자 
    boonmo = diff + 1  #분모
else :  # 라인이 홀수번째 일 때
    boonja = diff + 1  #분자
    boonmo = line - diff  #분모
print(boonja, '/', boonmo, sep='')

```


### Example:
<img width="1199" alt="스크린샷 2023-02-11 오전 4 10 13" src="https://user-images.githubusercontent.com/107760647/218177304-74acdd09-f492-4f38-8de9-10707dc8f4eb.png">


Reference:
https://www.acmicpc.net/problem/1193
