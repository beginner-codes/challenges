# Challenge 470 - Nearest Chapter

Create a function that returns which chapter is nearest to the page you're on. If two chapters are equidistant, return the chapter with the higher page number.

## Examples
```python
nearest_chapter({
  "Chapter 1" : 1,
  "Chapter 2" : 15,
  "Chapter 3" : 37
}, 10) ➞ "Chapter 2"


nearest_chapter({
  "New Beginnings" : 1,
  "Strange Developments" : 62,
  "The End?" : 194,
  "The True Ending" : 460
}, 200) ➞ "The End?"


nearest_chapter({
  "Chapter 1a" : 1,
  "Chapter 1b" : 5
}, 3) ➞ "Chapter 1b"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def nearest_chapter(chapters: dict[str, int], page: int) -> str:
    return ""  # Put your code here!!!


test(470, nearest_chapter)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            {
                "Chapter 1": 1,
                "Chapter 2": 15,
                "Chapter 3": 37
            },
            10
        ],
        "return": "Chapter 2"
    },
    {
        "args": [
            {
                "New Beginnings": 1,
                "Strange Developments": 62,
                "The End?": 194,
                "The True Ending": 460
            },
            200
        ],
        "return": "The End?"
    },
    {
        "args": [
            {
                "Chapter 1a": 1,
                "Chapter 1b": 5
            },
            3
        ],
        "return": "Chapter 1b"
    },
    {
        "args": [
            {
                "Chapter 1a": 1,
                "Chapter 1b": 5,
                "Chapter 1c": 50,
                "Chapter 1d": 100
            },
            75
        ],
        "return": "Chapter 1d"
    },
    {
        "args": [
            {
                "Chapter 1a": 1,
                "Chapter 1b": 5,
                "Chapter 1c": 50,
                "Chapter 1d": 100,
                "Chapter 1e": 200
            },
            150
        ],
        "return": "Chapter 1e"
    }
]
```
## Credits

Found on Edabit: [Nearest Chapter](https://edabit.com/challenge/ZeeWN5NdFa8ALJq5G)
