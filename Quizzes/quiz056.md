# Quiz056

## 1. Solution
```.py
class Handshake:
    def __init__(self, num: int):
        self.num = num

    def binary_convert(self):
        num_copy = self.num
        output = ""
        while num_copy > 1:
            if num_copy % 2 == 1:
                output = '1' + output
            else:
                output = '0' + output
            num_copy //= 2
        output = '1' + output

        while len(output) < 5:
            output = '0' + output

        return output

    def get_handshake(self):
        binary = self.binary_convert()
        actions = ['wink', 'double blink', 'close your eyes', 'jump']
        handshake = []
        for digit, action in zip(binary[::-1], actions):
            if digit == '1':
                handshake.append(action)
        if binary[0] == '1':
            handshake.reverse()
        return ", ".join(handshake)


t = Handshake(9)
print(t.get_handshake())

```
## 2. Proof of Work
![Quiz056](https://github.com/AntGra25/unit4-CS24/assets/142757981/4f6dffe9-3614-4764-8f66-1943a4957464)

## 3. 
