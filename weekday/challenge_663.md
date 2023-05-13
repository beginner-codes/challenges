# Challenge 663 - Gaderypoluki Cipher

Create a function that takes an encryption key (a string with an even number of characters) and a message to encrypt. Group the letters of the key by two:
```python
"gaderypoluki" -> "ga de ry po lu ki"
```
Now take the message for encryption. If the message character appears in the key, replace it with an adjacent character in the grouped version of the key. If the message character does not appear in the key, leave it as is. If the letter in the key occurs more than once, the first result is used. For example: use the above key, if the letter `"a"` appeared in the message, it would be replaced with `"g"` since `"g"` in the adjacent letter.

Return the encrypted message.

## Examples
```python
encrypt("ab c", "abc ab") ➞ "ba cba"

encrypt("otorhinolaryngological", "My name is Paul") ➞ "Mr olme hs Plua"

encrypt("gaderypoluki", "This is an encrypted message") ➞ "Thks ks gn dncyrotde mdssgad"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def encrypt(key: str, message: str) -> str:
    return ""  # Put your code here!!!


test(663, encrypt)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "ab c",
            "abc ab"
        ],
        "return": "ba cba"
    },
    {
        "args": [
            "gaderypoluki",
            "This is an encrypted message"
        ],
        "return": "Thks ks gn dncyrotde mdssgad"
    },
    {
        "args": [
            "otorhinolaryngological",
            "My name is Paul"
        ],
        "return": "Mr olme hs Plua"
    },
    {
        "args": [
            "1234567890",
            "1029384756"
        ],
        "return": "2910473865"
    }
]
```
## Credits

Found on Edabit: [Gaderypoluki Cipher](https://edabit.com/challenge/4AzBbuPLxKfJd7aeG)
