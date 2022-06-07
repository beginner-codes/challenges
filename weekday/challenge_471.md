# Challenge 471 - Same Parity?

Create a function that takes a number as input and returns `True` if the sum of its digits has the same parity as the entire number. Otherwise, return `False`.

## Examples
```python
parity_analysis(243) ➞ True
# 243 is odd and so is 9 (2 + 4 + 3)

parity_analysis(12) ➞ False
# 12 is even but 3 is odd (1 + 2)

parity_analysis(3) ➞ True
# 3 is odd and 3 is odd and 3 is odd (3)
```
## Notes

- Parity is whether a number is even or odd. If the sum of the digits is even and the number itself is even, return `True`. The same goes if the number is odd and so is the sum of its digits.
- Single digits will obviously have the same parities.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def parity_analysis(number: int) -> bool:
    return False  # Put your code here!!!


test(471, parity_analysis)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            243
        ],
        "return": true
    },
    {
        "args": [
            12
        ],
        "return": false
    },
    {
        "args": [
            3
        ],
        "return": true
    },
    {
        "args": [
            5
        ],
        "return": true
    },
    {
        "args": [
            4
        ],
        "return": true
    },
    {
        "args": [
            3453
        ],
        "return": true
    },
    {
        "args": [
            0
        ],
        "return": true
    },
    {
        "args": [
            123456789
        ],
        "return": true
    },
    {
        "args": [
            987654321
        ],
        "return": true
    },
    {
        "args": [
            13
        ],
        "return": false
    },
    {
        "args": [
            37
        ],
        "return": false
    },
    {
        "args": [
            182
        ],
        "return": false
    },
    {
        "args": [
            133331
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Same Parity?](https://edabit.com/challenge/jzCGNwLpmrHQKmtyJ)
