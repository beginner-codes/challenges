# Challenge 709 - Imaginary Coding Interview

Create a function to check if a candidate is qualified in an imaginary coding interview of an imaginary tech startup.

The criteria for a candidate to be qualified in the coding interview is:

- The candidate should have completed all the questions.
- The maximum time given to complete the interview is 120 minutes.
- The maximum time given for very easy questions is 5 minutes each.
- The maximum time given for easy questions is 10 minutes each.
- The maximum time given for medium questions is 15 minutes each.
- The maximum time given for hard questions is 20 minutes each.

- If all the above conditions are satisfied, return `"qualified"`, otherwise return `"disqualified"`.

You will be given a list of times taken by a candidate to solve each question and the total time taken by the candidate to complete the interview.

The list of times given will be for questions in the following order of difficulty `[very easy, very easy, easy, easy, medium, medium, hard, hard]`.

## Examples
```python
interview([5, 5, 10, 10, 15, 15, 20, 20], 120) ➞ "qualified"

interview([2, 3, 8, 6, 5, 12, 10, 18], 64) ➞  "qualified"

interview([5, 5, 10, 10, 25, 15, 20, 20], 120) ➞ "disqualified"
# Exceeded the time limit for a medium question.

interview([5, 5, 10, 10, 15, 15, 20], 120) ➞ "disqualified"
# Did not complete all the questions.

interview([5, 5, 10, 10, 15, 15, 20, 20], 130) ➞ "disqualified"
# Solved all the questions in their respected time limits but exceeded the total time limit of the interview.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def interview(question_times: list[int], total_time: int) -> str:
    return ""  # Put your code here!!!


test(709, interview)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                5,
                5,
                10,
                20,
                15,
                15,
                20,
                20
            ],
            140
        ],
        "return": "disqualified"
    },
    {
        "args": [
            [
                5,
                5,
                10,
                10,
                25,
                15,
                20,
                20
            ],
            120
        ],
        "return": "disqualified"
    },
    {
        "args": [
            [
                10,
                10,
                15,
                15,
                20,
                20
            ],
            150
        ],
        "return": "disqualified"
    },
    {
        "args": [
            [
                5,
                5,
                10,
                10,
                15,
                20,
                50
            ],
            160
        ],
        "return": "disqualified"
    },
    {
        "args": [
            [
                5,
                5,
                10,
                10,
                15,
                15,
                20,
                20
            ],
            120
        ],
        "return": "qualified"
    }
]
```
## Credits

Found on Edabit: [Imaginary Coding Interview](https://edabit.com/challenge/3A3mHS5B3NNZddQL2)
