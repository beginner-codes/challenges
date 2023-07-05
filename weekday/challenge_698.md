# Challenge 698 - Convert "Zero" and "One" to "1" and "0"

Create a function that takes a string as an argument. The function must return a string containing 1s and 0s based on the string argument's words. If any word in the argument is not equal to `"zero"` or `"one"` (case insensitive), you should ignore it. The returned string's length should be a multiple of 8, if the string is not a multiple of 8 you should remove the numbers in excess.

## Examples
```python
text_to_binary("zero one zero one zero one zero one") ➞ "01010101"

text_to_binary("Zero one zero ONE zero one zero one") ➞ "01010101"

text_to_binary("zero one zero one zero one zero one one two") ➞ "01010101"

text_to_binary("zero one zero one zero one zero three") ➞ ""

text_to_binary("one one") ➞ ""
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def text_to_binary(text: str) -> str:
    return ""  # Put your code here!!!


test(698, text_to_binary)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "one zero one"
        ],
        "return": ""
    },
    {
        "args": [
            "TWO one zero one one zero one zero"
        ],
        "return": ""
    },
    {
        "args": [
            "TWO one zero one one zero one zero one"
        ],
        "return": "10110101"
    },
    {
        "args": [
            "One zero zero one zero one one one zero one one zero zero zero zero one zero one one one zero one one zero zero zero zero one zero one one one zero one one zero zero zero zero one zero one one one zero one one zero zero zero zero one zero one one one zero one one zero zero zero zero one zero"
        ],
        "return": "1001011101100001011101100001011101100001011101100001011101100001"
    },
    {
        "args": [
            "one Zero zero one zero zero one one one one one zero oNe one one zero one zerO"
        ],
        "return": "1001001111101110"
    }
]
```
## Credits

Found on Edabit: [Convert "Zero" and "One" to "1" and "0"](https://edabit.com/challenge/i98e9Czup3kbfoHm3)
