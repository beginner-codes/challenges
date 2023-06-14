# Challenge 684 - Flipping Bits

You will be given a 32-bit unsigned integer. Flip all the bits 1 -> 0 and 0 -> 1 and return the result as an unsigned integer.


## Worked Example
```
n = 4
4 is 0100 in binary. We are working in 32 bits so:
00000000000000000000000000000100 = 4
11111111111111111111111111111011 = 4294967291
return 4294967291
```
## Examples
```python
flipping_bits(2147483647) ➞ 2147483648

flipping_bits(1) ➞ 4294967294

flipping_bits(4) ➞ 4294967291
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def flipping_bits(number: int) -> int:
    return 0  # Put your code here!!!


test(684, flipping_bits)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            2147483647
        ],
        "return": 2147483648
    },
    {
        "args": [
            35601423
        ],
        "return": 4259365872
    },
    {
        "args": [
            802743475
        ],
        "return": 3492223820
    },
    {
        "args": [
            0
        ],
        "return": 4294967295
    },
    {
        "args": [
            1
        ],
        "return": 4294967294
    }
]

```
## Credits

Found on Edabit: [Flipping Bits](https://edabit.com/challenge/z39yXccJGLAy3BDNX)
