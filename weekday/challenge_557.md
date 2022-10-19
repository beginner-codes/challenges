# Challenge 557 - Blah, Blah, Blah...

Create a function which replaces the last `n` words with `"blah"`. Add `"..."` to the last blah.

## Examples
```python
blah_blah("A function is a block of code which only runs when it is called",  5) ➞ "A function is a block of code which only blah blah blah blah blah..."

blah_blah("one two three four five", 2) ➞ "one two three blah blah..."

blah_blah("Sphinx of black quartz judge my vow", 10) ➞ "blah blah blah blah blah blah blah..."
```
## Notes

- If `n` is longer than the amount of words in the sentence, replace every word with `"blah"` (see example #3).
- All blahs shall be lowercase!

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def blah_blah(sentence: str, blahs: int) -> str:
    return "" # Put your code here!!!


test(557, blah_blah)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "Sphinx of black quartz judge my vow",
            10
        ],
        "return": "blah blah blah blah blah blah blah..."
    },
    {
        "args": [
            "one two three four five",
            2
        ],
        "return": "one two three blah blah..."
    },
    {
        "args": [
            "A function is a block of code which only runs when it is called",
            5
        ],
        "return": "A function is a block of code which only blah blah blah blah blah..."
    },
    {
        "args": [
            "The quadratic formula is negative b plus or minus the square root of b squared subtract four ac all over two a",
            5
        ],
        "return": "The quadratic formula is negative b plus or minus the square root of b squared subtract four blah blah blah blah blah..."
    }
]
```
## Credits

Found on Edabit: [Blah, Blah, Blah...](https://edabit.com/challenge/DnDLacMAgrxrq8mc3)
