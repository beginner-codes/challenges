# Challenge 552 - Substituting the The

Create a function that replaces `"the"` in the sentence with `"an"` or `"a"`. Remember that if the next word begins with a vowel, use `"an"`. In the case of a consonant, use `"a"`.

## Examples
```python
replace_the("the dog and the envelope") ➞ "a dog and an envelope"

replace_the("the boy ran at the wall") ➞ "a boy ran at a wall"

replace_the("the egg, the spoon and the espionage") ➞ "an egg, a spoon and an espionage"
```
## Notes

- Sentences will always be in lowercase.
- The last word of the sentence will never be `"the"`.
- This won't cover edge cases such as `"an hour"` or `"a unique thing"` (since they sound differently to the rule).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def replace_the(string: str) -> str:
    return "" # Put your code here!!!


test(552, replace_the)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "the boy ran at the wall"
        ],
        "return": "a boy ran at a wall"
    },
    {
        "args": [
            "this edabit thing is quite neat"
        ],
        "return": "this edabit thing is quite neat"
    },
    {
        "args": [
            "the quick brown fox jumps over the lazy dog"
        ],
        "return": "a quick brown fox jumps over a lazy dog"
    },
    {
        "args": [
            "the lion, witch and the wardrobe"
        ],
        "return": "a lion, witch and a wardrobe"
    },
    {
        "args": [
            "enter the correct password to access the epic program"
        ],
        "return": "enter a correct password to access an epic program"
    },
    {
        "args": [
            "this the random english sentence which you have to pass"
        ],
        "return": "this a random english sentence which you have to pass"
    },
    {
        "args": [
            "the dog and the envelope"
        ],
        "return": "a dog and an envelope"
    },
    {
        "args": [
            "where is the spoon"
        ],
        "return": "where is a spoon"
    },
    {
        "args": [
            "the egg, the spoon and the espionage"
        ],
        "return": "an egg, a spoon and an espionage"
    },
    {
        "args": [
            "the man blew the final candle out and all was dark"
        ],
        "return": "a man blew a final candle out and all was dark"
    },
    {
        "args": [
            "the ant ate the egg salad which the eel had been intending to eat over the weekend"
        ],
        "return": "an ant ate an egg salad which an eel had been intending to eat over a weekend"
    }
]
```
## Credits

Found on Edabit: [Substituting the The](https://edabit.com/challenge/JPfqYkt6KGhpwfYK7)
