# Challenge 520 - Even or Odd: Which is Greater?

Create a function to determine if the sum of all the individual even digits are greater than the sum of all the individual odd digits in a string of numbers.

- If the sum of odd numbers is greater than the sum of even numbers, return `"Odd is greater than Even"`.
- If the sum of even numbers is greater than the odd numbers, return `"Even is greater than Odd"`.
- If the sum of both even and odd numbers are equal, return `"Even and Odd are the same"`.

## Examples
```python
even_or_odd("22471") ➞ "Even and Odd are the same"

even_or_odd("213613") ➞ "Even and Odd are the same"

even_or_odd("23456") ➞ "Even is greater than Odd"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def even_or_odd(numbers: str) -> str:
    return "" # Put your code here!!!


test(520, even_or_odd)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "14256"
        ],
        "return": "Even is greater than Odd"
    },
    {
        "args": [
            "123"
        ],
        "return": "Odd is greater than Even"
    },
    {
        "args": [
            "112"
        ],
        "return": "Even and Odd are the same"
    },
    {
        "args": [
            "124"
        ],
        "return": "Even is greater than Odd"
    },
    {
        "args": [
            "6721"
        ],
        "return": "Even and Odd are the same"
    },
    {
        "args": [
            "23456"
        ],
        "return": "Even is greater than Odd"
    },
    {
        "args": [
            "92184"
        ],
        "return": "Even is greater than Odd"
    },
    {
        "args": [
            "45228"
        ],
        "return": "Even is greater than Odd"
    },
    {
        "args": [
            "143"
        ],
        "return": "Even and Odd are the same"
    },
    {
        "args": [
            "12378"
        ],
        "return": "Odd is greater than Even"
    }
]
```
## Credits

Found on Edabit: [Even or Odd: Which is Greater?](https://edabit.com/challenge/suhHcPgaKdb9YCrve)
