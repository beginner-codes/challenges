# Challenge 707 - Words that Start with a Vowel

Write a function that retrieves all words that begin with a vowel.

## Examples
```python
retrieve("A simple life is a happy life for me.") ➞ ["a", "is", "a"]

retrieve("Exercising is a healthy way to burn off energy.")
➞ ["exercising", "is", "a", "off", "energy"]

retrieve("The poor ostrich was ostracized.")
➞ ["ostrich", "ostracized"]

retrieve("")
➞ []
```
## Notes

- Make all words lower case in the output.
- Retrieve the words in the order they appear in the sentence.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def retrieve(sentence: str) -> list[str]:
    return []  # Put your code here!!!


test(707, retrieve)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "The poor ostrich was ostracized."
        ],
        "return": [
            "ostrich",
            "ostracized"
        ]
    },
    {
        "args": [
            ""
        ],
        "return": []
    },
    {
        "args": [
            "Exercising is a healthy way to burn off energy."
        ],
        "return": [
            "exercising",
            "is",
            "a",
            "off",
            "energy"
        ]
    },
    {
        "args": [
            "A simple life is a happy life for me."
        ],
        "return": [
            "a",
            "is",
            "a"
        ]
    }
]
```
## Credits

Found on Edabit: [Words that Start with a Vowel](https://edabit.com/challenge/Dm7iqogzdGJTsaHZg)
