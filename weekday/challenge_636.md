# Challenge 636 - First Tuesday of the Month

Every month, Microny™️ publishes a few free video games on their website. You are working on a script that will notify you whenever the new games are available for download. There is not a fixed date for the new releases, but you know that it happens on the first Tuesday of every month.

Write a function that, given a year and a month, returns a string with the date of when the new games will be available.

## Examples
```python
first_tuesday_of_the_month(1997, 1) ➞ "1997-01-07"

first_tuesday_of_the_month(2021, 2) ➞ "2021-02-02"

first_tuesday_of_the_month(2020, 3) ➞ "2020-03-03"
```
## Notes

- Months are given as numbers starting at `1 = January`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def first_tuesday_of_the_month(year: int, month: int) -> str:
    return ""  # Put your code here!!!


test(636, first_tuesday_of_the_month)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            2021,
            2
        ],
        "return": "2021-02-02"
    },
    {
        "args": [
            2009,
            6
        ],
        "return": "2009-06-02"
    },
    {
        "args": [
            1992,
            5
        ],
        "return": "1992-05-05"
    },
    {
        "args": [
            1987,
            7
        ],
        "return": "1987-07-07"
    },
    {
        "args": [
            2020,
            9
        ],
        "return": "2020-09-01"
    }
]
```
## Credits

Found on Edabit: [First Tuesday of the Month](https://edabit.com/challenge/GZ5gCe5jnbNRWqc5J)
