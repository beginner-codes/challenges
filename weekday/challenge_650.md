# Challenge 650 - Sort Numbers in Descending Order

Create a function that takes any non-negative number as an argument and returns it with its digits in descending order.

## Examples
```python
sort_descending(123) ➞ 321

sort_descending(1254859723) ➞ 9875543221

sort_descending(73065) ➞ 76530
```
## Notes

- You can expect non-negative numbers for all test cases.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sort_descending(number: int) -> int:
    return 0  # Put your code here!!!


test(650, sort_descending)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            444111888555333
        ],
        "return": 888555444333111
    },
    {
        "args": [
            123
        ],
        "return": 321
    },
    {
        "args": [
            628904
        ],
        "return": 986420
    },
    {
        "args": [
            670276097
        ],
        "return": 977766200
    },
    {
        "args": [
            81294
        ],
        "return": 98421
    }
]
```
## Credits

Found on Edabit: [Sort Numbers in Descending Order](https://edabit.com/challenge/B7rfWiJKrwft9yXXC)
