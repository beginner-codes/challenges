# Challenge 630 - Super Reduced String

Steve has a string of lowercase characters in range a-z. He wants to reduce the string to its shortest length by doing a series of operations. In each operation, he selects a pair of adjacent lowercase letters that match, and he deletes them. For instance, the string `aab` could be shortened to `b` in one operation.

Steve’s task is to delete as many characters as possible using this method and print the resulting string. If the final string is empty, return `"Empty String"`.

## Case
```python
super_reduced_string("aaabccddd") ➞ "abd"
```
## Explanation:
```python
"aaabccddd" -> "abccddd" -> "abddd" -> "abd"
```
## Examples
```python
super_reduced_string("cccxllyyy") ➞ "cxy"

super_reduced_string("aa") ➞ "Empty String"

super_reduced_string("baab") ➞ "Empty String"

super_reduced_string("fghiiijkllmnnno") ➞ "fghijkmno"

super_reduced_string("chklssstt") ➞ "chkls"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def super_reduced_string(string: str) -> str:
    return ""  # Put your code here!!!


test(630, super_reduced_string)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "zzzhhnnttti"
        ],
        "return": "zti"
    },
    {
        "args": [
            "bccddb"
        ],
        "return": "Empty String"
    },
    {
        "args": [
            "abbccddfghiaklmno"
        ],
        "return": "afghiaklmno"
    },
    {
        "args": [
            "qqq"
        ],
        "return": "q"
    },
    {
        "args": [
            "acdqglrfkqyuqfjkxyqvnrtysfrzrmzlygfveulqfpdbhlqdqrrqdqlhbdpfqluevfgylzmrzrfsytrnvqyxkjfquyqkfrlacdqj"
        ],
        "return": "acdqgacdqj"
    }
]
```
## Credits

Found on Edabit: [Super Reduced String](https://edabit.com/challenge/JBTLDxvdzpjyJA4Nv)
