# Challenge 727 - Hamming Code

A Hamming Code is used to correct errors in data transmissions. Create a function that takes a string containing the message and returns an encoded message using hamming code.

There are some variations on the rules for enciphering. One version of the cipher rules are outlined below:
```python
hamming_code("hey") ➞
"000111111000111000000000000111111000000111000111000111111111111000000111"
```
1. Convert every character to its ASCII value:
```python
h, e, y = 104, 101, 121
```
2. Convert ASCII values to 8-bit binary:
```python
104, 101, 121 = 01101000, 01100101, 01111001
```
3. Triple every bit:
```python
01101000, 01100101, 01111001 =

000111111000111000000000, 000111111000000111000111, 000111111111111000000111
```
4. Concatenate the result:
```python
"000111111000111000000000000111111000000111000111000111111111111000000111"
```
See the below examples for a better understanding:

Examples
```python
hamming_code("hey") ➞
"000111111000111000000000000111111000000111000111000111111111111000000111"

hamming_code("coding") ➞
"000111111000000000111111000111111000111111111111000111111000000111000000000111111000111000000111000111111000111111111000000111111000000111111111"

hamming_code("matt") ➞
"000111111000111111000111000111111000000000000111000111111111000111000000000111111111000111000000"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def hamming_code(message: str) -> str:
    return ""  # Put your code here!!!


test(727, hamming_code)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "hey"
        ],
        "return": "000111111000111000000000000111111000000111000111000111111111111000000111"
    },
    {
        "args": [
            "matt"
        ],
        "return": "000111111000111111000111000111111000000000000111000111111111000111000000000111111111000111000000"
    },
    {
        "args": [
            "T?st!%"
        ],
        "return": "000111000111000111000000000000111111111111111111000111111111000000111111000111111111000111000000000000111000000000000111000000111000000111000111"
    },
    {
        "args": [
            "coding"
        ],
        "return": "000111111000000000111111000111111000111111111111000111111000000111000000000111111000111000000111000111111000111111111000000111111000000111111111"
    },
    {
        "args": [
            "T3st"
        ],
        "return": "000111000111000111000000000000111111000000111111000111111111000000111111000111111111000111000000"
    }
]

```
## Credits

Found on Edabit: [Hamming Code](https://edabit.com/challenge/HNjRjrNPueF5vRh9S)
