## Question 2753

### There are 3 conditions to get 윤년

* 4의 배수
* 100의 배수가 아닌 것
* 400의 배수

```python 3
yr = int(input())

if ((yr%4 == 0)and(yr%100 != 0)) or (yr%400 == 0):
    print('1')
else:
    print('0')
```


### Example:
<img width="1186" alt="스크린샷 2023-01-16 오전 5 59 18" src="https://user-images.githubusercontent.com/107760647/212566978-40fa4906-9f71-407b-9d50-7439782a9c72.png">


Reference:
https://www.acmicpc.net/problem/2753

