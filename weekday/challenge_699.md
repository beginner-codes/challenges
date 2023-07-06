# Challenge 699 - When Will You Save a Million?

You landed your dream job. They pay in geometric progression. In your first month of work, you will get your first paycheck. For every month after, your paycheck will be a multiplier times bigger than the previous paycheck.

Create a function that takes the first month's paycheck and the multiplier and returns the number of months it would take for you to save up more than one million. The problem assumes you save 100% of every paycheck.

## Examples
```python
months_to_million(10, 2) ➞ 17

months_to_million(100, 1.01) ➞ 464

months_to_million(50, 100) ➞ 4
# Month 1 = 50 (paycheck 50)
# Month 2 = 5050 (paycheck 5,000 + 50 already saved)
# Month 3 = 505050 (paycheck 500,000 + 5,050 already saved)
# Month 4 = 50505050 (paycheck 50,000,000 + 505,050 already saved)
```
## Notes

- Don't forget to return the result in the number of months.
- Return when your savings are greater than 1,000,000.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def months_to_million(first_month: int, multiplier: int) -> int:
    return 0  # Put your code here!!!


test(699, months_to_million)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            5,
            2
        ],
        "return": 18
    },
    {
        "args": [
            1,
            2
        ],
        "return": 20
    },
    {
        "args": [
            1,
            1.01
        ],
        "return": 926
    },
    {
        "args": [
            4,
            2
        ],
        "return": 18
    },
    {
        "args": [
            11,
            11
        ],
        "return": 6
    }
]
```
## Credits

Found on Edabit: [When Will You Save a Million?](https://edabit.com/challenge/n4JA3je7FEFfZKaWp)
