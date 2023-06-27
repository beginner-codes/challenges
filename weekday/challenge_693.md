# Challenge 693 - Pronouncing the Xs

Create a function which replaces all the x's in the string in the following ways:

- Replace x's at the start of a word with `"z"`.
- Replace x with `"ecks"` if the word is only the x.
- Otherwise, replace all x's with `"cks"`

## Examples
```python
x_pronounce("Inside the box was a xylophone") ➞ "Inside the bocks was a zylophone"

x_pronounce("The x ray is excellent") ➞ "The ecks ray is eckscellent"

x_pronounce("OMG x box unboxing video x D") ➞ "OMG ecks bocks unbocksing video ecks D"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def x_pronounce(sentence: str) -> str:
    return ""  # Put your code here!!!


test(693, x_pronounce)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "xerxes"
        ],
        "return": "zerckses"
    },
    {
        "args": [
            "Inside the box was a xylophone"
        ],
        "return": "Inside the bocks was a zylophone"
    },
    {
        "args": [
            "OMG xylem unboxing video x D"
        ],
        "return": "OMG zylem unbocksing video ecks D"
    },
    {
        "args": [
            "Anti vax"
        ],
        "return": "Anti vacks"
    },
    {
        "args": [
            "I gotta make bux but the clox are ticking!"
        ],
        "return": "I gotta make bucks but the clocks are ticking!"
    }
]
```
## Credits

Found on Edabit: [Pronouncing the Xs](https://edabit.com/challenge/bfz7kTgPujtfcHR9d)
