## Question 5622


```python 3
num = input()
time = 0
for i in num:
    if i in ['A', 'B', 'C']:
        time += 3
    elif i in ['D', 'E', 'F']:
        time += 4
    elif i in ['G', 'H', 'I']:
        time += 5
    elif i in ['J', 'K', 'L']:
        time += 6
    elif i in ['M', 'N', 'O']:
        time += 7
    elif i in ['P', 'Q', 'R', 'S']:
        time += 8
    elif i in ['T', 'U', 'V']:
        time += 9
    elif i in ['W', 'X', 'Y', 'Z']:
        time += 10
print(time)

```


### Example:
<img width="1212" alt="스크린샷 2023-02-03 오전 5 09 38" src="https://user-images.githubusercontent.com/107760647/216438749-3c9a9dca-d1ce-4b67-ac93-0e25dc5da922.png">


Reference:
https://www.acmicpc.net/problem/5622
