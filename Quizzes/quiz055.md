# Quiz055

## 1. Solution
```
import math

class darts:
    def points(self, x: float, y: float) -> int:
        distance = math.sqrt(x**2 + y**2)
        if distance > 10:
            return 0
        elif distance > 5:
            return 1
        elif distance > 1:
            return 5
        else:
            return 10


dart = darts()
print(dart.points(-0.5, 0.5))
print(dart.points(4, 3))
print(dart.points(6, 8))
print(dart.points(11, 11))

```

## 2. Proof of Work
![Quiz055](https://github.com/AntGra25/unit4-CS24/assets/142757981/2311c499-fc48-40f6-bb0a-c0ce2875607b)

## 3. 
