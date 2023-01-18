## Question 2884

```python 3

H,M = map(int,input().split())

if M < 45 :
    if H == 0 :
        H = 23
        M += 60
    else :
        H -= 1
        M += 60
        
print(H, M-45)



# ------------------- or -------------- #
H,M = map(int,input().split())

if M > 44:
    print(H,M-45),
elif H > 0 and M < 45:
    print(H-1, M+15),
else:
    print(23, M+15)
```


### Example:
<img width="1198" alt="스크린샷 2023-01-19 오전 5 53 46" src="https://user-images.githubusercontent.com/107760647/213292340-bef7d083-9cb0-4a83-9355-9aacb21ed42a.png">


Reference:
https://www.acmicpc.net/problem/2884

