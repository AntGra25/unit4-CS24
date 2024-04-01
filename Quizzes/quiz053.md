# Quiz053

## 1. Solution
```.py
class palNum:
    def __init__(self, A: int, B: int):
        self.A = A
        self.B = B

    def get_pal_list(self):
        pal_list = []
        for i in range(self.A, self.B + 1):
            if str(i) == str(i)[::-1]:
                pal_list.append(i)
        return pal_list


pals1 = palNum(A=1, B=9)
pals2 = palNum(A=10, B=199)
print(pals1.get_pal_list())
print(pals2.get_pal_list())

```
## 2. Proof of Work
![Quiz053](https://github.com/AntGra25/unit4-CS24/assets/142757981/033d6f5f-0064-448c-ab41-b160d727e6c5)

## 3. 
