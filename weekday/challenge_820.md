# Challenge 820 - Calculated Bonus

A financial institution provides professional services to banks and claims charges from the customers based on the number of man-days provided. Internally, it has set a scheme to motivate and reward staff to meet and exceed targeted billable utilization and revenues by paying a bonus for each day claimed from customers in excess of a threshold target.

This quarterly scheme is calculated with a threshold target of 32 days per quarter, and the incentive payment for each billable day in excess of such threshold target is shown as follows:
```
Days                    Bonus
0 to 32 days            Zero
33 to 40 days           SGD$325 per billable day
41 to 48 days           SGD$550 per billable day
Greater than 48 days    SGD$600 per billable day
```
Please note that incentive payment is calculated progressively. As an example, if an employee reached total billable days of 45 in a quarter, his/her incentive payment is computed as follows:
```
32*0 + 8*325 + 5*550 = 5350
```
Write a function to read the billable days of an employee and return the bonus he/she has obtained in that quarter.

## Examples
```python
bonus(15) ➞ 0

bonus(37) ➞ 1625

bonus(50) ➞ 8200
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def bonus(billable_days: int) -> int:
    return 0  # Put your code here!!!


test(820, bonus)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            37
        ],
        "return": 1625
    },
    {
        "args": [
            50
        ],
        "return": 8200
    },
    {
        "args": [
            15
        ],
        "return": 0
    }
]
```

## Credits

Found on Edabit: [Calculated Bonus](https://edabit.com/challenge/ksiA6Q34iXgTcMeZF)
