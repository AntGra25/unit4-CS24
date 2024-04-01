# Quiz054

## 1. Solution
```.py
class rainDrops:
    def pour(self, n: int) -> str:
        result = ""
        if n % 3 == 0:
            result += "Pling"
        if n % 5 == 0:
            result += "Plang"
        if n % 7 == 0:
            result += "Plong"
        if result == "":
            result = str(n)
        return result


rain = rainDrops()
print(rain.pour(28))
print(rain.pour(30))
print(rain.pour(34))

```
## 2. Proof of Work
![image](https://github.com/AntGra25/unit4-CS24/assets/142757981/cc33fba4-47c3-4594-b61a-f983f1ab455d)

## 3. UML Diagram
![Quiz054C](https://github.com/AntGra25/unit4-CS24/assets/142757981/204a2eab-b5d6-439d-8d57-37c18177258c)

