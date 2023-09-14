# Challenge 750 - Rhyme Time

Create a function that returns `True` if two lines rhyme and `False` otherwise. For the purposes of this exercise, two lines rhyme if the last word from each sentence contains the same vowels.

## Examples
```python
does_rhyme("Sam I am!", "Green eggs and ham.") ➞ True

does_rhyme("Sam I am!", "Green eggs and HAM.") ➞ True
# Capitalization and punctuation should not matter.

does_rhyme("You are off to the races", "a splendid day.") ➞ False

does_rhyme("and frequently do?", "you gotta move.") ➞ False
```
## Notes

- We are ignoring cases like "thyme" and "lime".
- We are also ignoring cases like "away" and "today" (which technically rhyme, even though they contain different vowels).

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


def does_rhyme(sentence_a: str, sentence_b: str) -> bool:
    return False  # Put your code here!!!


test(750, does_rhyme)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "you will start to race",
            "the waiting Place"
        ],
        "return": true
    },
    {
        "args": [
            "down by the bay",
            "where the watermelons grow"
        ],
        "return": false
    },
    {
        "args": [
            "head straight to town",
            "give me not a frown"
        ],
        "return": true
    },
    {
        "args": [
            "Sam I am!",
            "Green eggs and ham."
        ],
        "return": true
    },
    {
        "args": [
            "and frequently do?",
            "you gotta move."
        ],
        "return": false
    }
]
```

## Credits

Found on Edabit: [Rhyme Time](https://edabit.com/challenge/jwiJNMiCW6P5d2XXA)
