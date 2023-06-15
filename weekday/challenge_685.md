# Challenge 685 - Palindromic Anagrams

Given a word, create a function which returns whether it's possible to create a palindrome by rearranging the letters in the word.

## Examples
```python
is_palindrome_possible("rearcac") ➞ True
# You can make "racecar"

is_palindrome_possible("suhbeusheff") ➞ True
# You can make "sfuehbheufs" (not a real word but still a palindrome)

is_palindrome_possible("palindrome") ➞ False
# It's impossible
```
## Notes

- Trivially, words which are already palindromes return `True`.
- Words are given in all lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def is_palindrome_possible(word: str) -> bool:
    return False  # Put your code here!!!


test(685, is_palindrome_possible)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "hfe"
        ],
        "return": false
    },
    {
        "args": [
            "wow"
        ],
        "return": true
    },
    {
        "args": [
            "arrad"
        ],
        "return": true
    },
    {
        "args": [
            "zgzqxljjp"
        ],
        "return": false
    },
    {
        "args": [
            "reparpe"
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Palindromic Anagrams](https://edabit.com/challenge/eyJ4mN6RpyiRTvSob)
