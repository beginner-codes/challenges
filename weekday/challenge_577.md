# Challenge 577 - Reverse the Order of Words with Five Letters or More

Write a function that takes a string of one or more words as an argument and returns the same string, but with all five or more letter words reversed. Strings passed in will consist of only letters and spaces. Spaces will be included only when more than one word is present.

## Examples
```python
reverse_long_words("Reverse") ➞ "esreveR"

reverse_long_words("This is a typical sentence.") ➞ "This is a lacipyt .ecnetnes"

reverse_long_words("The dog is big.") ➞ "The dog is big."
```
## Notes

- You can expect a valid string to be provided for each test case.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def reverse_long_words(string: str) -> str:
    return ""  # Put your code here!!!


test(577, reverse_long_words)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "The old apple revels in its authority."
        ],
        "return": "The old elppa slever in its .ytirohtua"
    },
    {
        "args": [
            "Reverse"
        ],
        "return": "esreveR"
    },
    {
        "args": [
            "Please wait outside of the house."
        ],
        "return": "esaelP wait edistuo of the .esuoh"
    },
    {
        "args": [
            "Two seats were vacant."
        ],
        "return": "Two staes were .tnacav"
    },
    {
        "args": [
            "The dog is big."
        ],
        "return": "The dog is big."
    }
]
```
## Credits

Found on Edabit: [Reverse the Order of Words with Five Letters or More](https://edabit.com/challenge/uS8tMvEyvTXD88wps)
