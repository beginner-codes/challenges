# Challenge 677 - First Letter Shift

Given a sentence, create a function which shifts the first letter of each word to the next word in the sentence (shifting right).

## Examples
```python
shift_sentence("create a function") ➞ "freate c aunction"

shift_sentence("it should shift the sentence") ➞ "st ihould shift she tentence"

shift_sentence("the output is not very legible") ➞ "lhe tutput os iot nery vegible"

shift_sentence("programming") ➞ "programming"
```
## Notes

- The last word shifts its first letter to the first word in the sentence.
- All sentences will be given in lowercase.
- Note how single words remain untouched.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def shift_sentence(sentence: str) -> str:
    return ""  # Put your code here!!!


test(677, shift_sentence)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "programming"
        ],
        "return": "programming"
    },
    {
        "args": [
            "tey ghis uot hnscrambled"
        ],
        "return": "hey this got unscrambled"
    },
    {
        "args": [
            "sarah the key is under the door mat"
        ],
        "return": "marah she tey ks inder uhe toor dat"
    },
    {
        "args": [
            "i love to eat scrambled eggs and ham"
        ],
        "return": "h iove lo tat ecrambled sggs end aam"
    },
    {
        "args": [
            "where is the butter"
        ],
        "return": "bhere ws ihe tutter"
    }
]
```
## Credits

Found on Edabit: [First Letter Shift](https://edabit.com/challenge/ojNRprg7fKpWJpj47)
