# Challenge 532 - Phone Number Word Decoder 

Create a program that converts a phone number with letters to one with only numbers.

Number to letter mapping:
```
Number	Letter
0	    none
1	    none
2	    ABC
3   	DEF
4	    GHI
5	    JKL
6	    MNO
7	    PQRS
8	    TUV
9	    WXYZ
```
## Examples
```python
text_to_num("123-647-EYES") ➞ "123-647-3937"

text_to_num("(325)444-TEST") ➞ "(325)444-8378"

text_to_num("653-TRY-THIS") ➞ "653-879-8447"

text_to_num("435-224-7613") ➞ "435-224-7613"
```
## Notes

- All inputs will be formatted as a string representing a proper phone number in the format `XXX-XXX-XXXX` or `(XXX)XXX-XXXX`, using numbers and capital letters.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def text_to_num(phone_number: str) -> str:
    return "" # Put your code here!!!


test(532, text_to_num)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": "(325)444-8378",
        "return": [
            "(325)444-TEST"
        ]
    },
    {
        "args": "(025)445-6741",
        "return": [
            "(025)445-6741"
        ]
    },
    {
        "args": "435-224-7613",
        "return": [
            "435-224-7613"
        ]
    },
    {
        "args": "653-879-8447",
        "return": [
            "653-TRY-THIS"
        ]
    },
    {
        "args": "123-647-3937",
        "return": [
            "123-647-EYES"
        ]
    }
]
```
## Credits

Found on Edabit: [Phone Number Word Decoder](https://edabit.com/challenge/nh3daaT8LHbv8mKXA)
