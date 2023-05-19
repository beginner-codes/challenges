# Challenge 667 - Any Prime Number in Range

Create a function that returns `True` if there's at least one prime number in the given range (start to end inclusive), `False` otherwise.

## Examples
```python
prime_in_range(10, 15) ➞ True
# Prime numbers in range: 11, 13

prime_in_range(62, 66) ➞ False
# No prime numbers in range.

prime_in_range(3, 5) ➞ True
# Prime numbers in range: 3, 5
```
## Notes

- `end` is always greater than `start`.
- `start` and `end` are always positive.
- 0 and 1 aren't prime numbers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def prime_in_range(start: int, end: int) -> bool:
    return False  # Put your code here!!!


test(667, prime_in_range)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            10,
            12
        ],
        "return": true
    },
    {
        "args": [
            62,
            66
        ],
        "return": false
    },
    {
        "args": [
            114,
            120
        ],
        "return": false
    },
    {
        "args": [
            441,
            445
        ],
        "return": true
    },
    {
        "args": [
            20,
            22
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Any Prime Number in Range](https://edabit.com/challenge/yFEMocjdiRjPhoDqv)
