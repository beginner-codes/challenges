# Challenge 460 - Premier League Champions

Create a function that takes a list of football clubs with properties: `name`, `wins`, `loss`, `draws`, `scored`, `conceded`, and returns the team name with the highest number of points. If two teams have the same number of points, return the team with the largest goal difference.

_How to Calculate Points and Goal Difference_
```python
team = { "name": "Manchester United", "wins": 30, "loss": 3, "draws": 5, "scored": 88, "conceded": 20 }

Total Points = 3 * wins + 0 * loss + 1 * draws = 3 * 30 + 0 * 3 + 5 * 1 = 95 points
Goal Difference = scored - conceded = 88 - 20 = 68
```
## Examples
```python
champions([
  {
    "name": "Manchester United",
    "wins": 30,
    "loss": 3,
    "draws": 5,
    "scored": 88,
    "conceded": 20,
  },
  {
    "name": "Arsenal",
    "wins": 24,
    "loss": 6,
    "draws": 8,
    "scored": 98,
    "conceded": 29,
  },
  {
    "name": "Chelsea",
    "wins": 22,
    "loss": 8,
    "draws": 8,
    "scored": 98,
    "conceded": 29,
  }
]) ➞ "Manchester United"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def champions(teams: list[dict]) -> str:
    return ""  # Put your code here!!!


test(460, champions())  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                {
                    "name": "Manchester United",
                    "wins": 30,
                    "loss": 3,
                    "draws": 5,
                    "scored": 88,
                    "conceded": 20
                },
                {
                    "name": "Arsenal",
                    "wins": 24,
                    "loss": 6,
                    "draws": 8,
                    "scored": 98,
                    "conceded": 29
                },
                {
                    "name": "Chelsea",
                    "wins": 22,
                    "loss": 8,
                    "draws": 8,
                    "scored": 98,
                    "conceded": 29
                }
            ]
        ],
        "return": "Manchester United"
    },
    {
        "args": [
            [
                {
                    "name": "Manchester City",
                    "wins": 30,
                    "loss": 8,
                    "draws": 0,
                    "scored": 67,
                    "conceded": 20
                },
                {
                    "name": "Liverpool",
                    "wins": 34,
                    "loss": 2,
                    "draws": 2,
                    "scored": 118,
                    "conceded": 29
                },
                {
                    "name": "Leicester City",
                    "wins": 22,
                    "loss": 8,
                    "draws": 8,
                    "scored": 98,
                    "conceded": 29
                }
            ]
        ],
        "return": "Liverpool"
    },
    {
        "args": [
            [
                {
                    "name": "Manchester City",
                    "wins": 30,
                    "loss": 8,
                    "draws": 0,
                    "scored": 67,
                    "conceded": 20
                },
                {
                    "name": "New Castle United",
                    "wins": 34,
                    "loss": 2,
                    "draws": 2,
                    "scored": 118,
                    "conceded": 36
                },
                {
                    "name": "Leicester City",
                    "wins": 34,
                    "loss": 2,
                    "draws": 2,
                    "scored": 108,
                    "conceded": 21
                }
            ]
        ],
        "return": "Leicester City"
    },
    {
        "args": [
            [
                {
                    "name": "Manchester City",
                    "wins": 30,
                    "loss": 6,
                    "draws": 2,
                    "scored": 102,
                    "conceded": 20
                },
                {
                    "name": "Liverpool",
                    "wins": 24,
                    "loss": 6,
                    "draws": 8,
                    "scored": 118,
                    "conceded": 29
                },
                {
                    "name": "Arsenal",
                    "wins": 28,
                    "loss": 2,
                    "draws": 8,
                    "scored": 87,
                    "conceded": 39
                }
            ]
        ],
        "return": "Manchester City"
    },
    {
        "args": [
            [
                {
                    "name": "Manchester City",
                    "wins": 30,
                    "loss": 6,
                    "draws": 2,
                    "scored": 102,
                    "conceded": 20
                },
                {
                    "name": "Liverpool",
                    "wins": 24,
                    "loss": 6,
                    "draws": 8,
                    "scored": 118,
                    "conceded": 29
                },
                {
                    "name": "Arsenal",
                    "wins": 30,
                    "loss": 0,
                    "draws": 8,
                    "scored": 87,
                    "conceded": 39
                }
            ]
        ],
        "return": "Arsenal"
    },
    {
        "args": [
            [
                {
                    "name": "Chelsea",
                    "wins": 35,
                    "loss": 3,
                    "draws": 0,
                    "scored": 102,
                    "conceded": 20
                },
                {
                    "name": "Liverpool",
                    "wins": 24,
                    "loss": 6,
                    "draws": 8,
                    "scored": 118,
                    "conceded": 29
                },
                {
                    "name": "Arsenal",
                    "wins": 28,
                    "loss": 2,
                    "draws": 8,
                    "scored": 87,
                    "conceded": 39
                }
            ]
        ],
        "return": "Chelsea"
    }
]
```
## Credits

Found on Edabit: [Premier League Champions](https://edabit.com/challenge/cToBLderwJrpqML8w)
