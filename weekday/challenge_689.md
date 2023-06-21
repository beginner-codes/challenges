# Challenge 689 - Triple + Double = So Much Trouble 

Create a function that takes two integers and returns `true` if a digit repeats three times in a row at any place in the first number AND that same digit repeats two times in a row in the second number.

## Examples
```python
trouble(451999277, 41177722899) ➞ True

trouble(1222345, 12345) ➞ False

trouble(666789, 12345667) ➞ True

trouble(33789, 12345337) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def trouble(number_one: int, number_two: int) -> bool:
    return False  # Put your code here!!!


test(689, trouble)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            9111922229333339,
            9559669779
        ],
        "return": false
    },
    {
        "args": [
            888,
            888
        ],
        "return": true
    },
    {
        "args": [
            451999277,
            41177722899
        ],
        "return": true
    },
    {
        "args": [
            1222345,
            12345
        ],
        "return": false
    },
    {
        "args": [
            12345,
            12345
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Triple + Double = So Much Trouble](https://edabit.com/challenge/CNpZrDFf3Ct7MzQrw)
