# Challenge 697 - Repeating Cycle

Given an integer, create a function that returns the length of the repeating cycle of the sequence `1/n`. If the cycle is non-repetitive, return `-1`.
```python
repeating_cycle(13) ➞ 6
# 1/13 = 0.076923 076923 076923 076923 ...
# length of `076923` is 6.
```
## Examples
```python
repeating_cycle(5) ➞ -1
# 1/5 = 0.2 (non-repeative)

repeating_cycle(33) ➞ 2
# 1/33 = 0.03 03 03 03 03 03 03 03
# length of `03` is 2

repeating_cycle(197) ➞ 98
```
## Notes

- Return `-1` if the repeating cycle does not start from the first decimal place. As an example, `1/22 = 0.0 45 45 45 45`, your function should return `-1` in this case.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def repeating_cycle(number: int) -> int:
    return 0  # Put your code here!!!


test(697, repeating_cycle)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            38127
        ],
        "return": 6230
    },
    {
        "args": [
            53
        ],
        "return": 13
    },
    {
        "args": [
            111
        ],
        "return": 3
    },
    {
        "args": [
            197
        ],
        "return": 98
    },
    {
        "args": [
            159
        ],
        "return": 13
    }
]
```
## Credits

Found on Edabit: [Repeating Cycle](https://edabit.com/challenge/x3t264gonaSRXT8GL)
