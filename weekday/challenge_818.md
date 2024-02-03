# Challenge 818 - Word Nests

A word nest is created by taking a starting word, and generating a new string by placing the word inside itself. This process is then repeated.

Nesting 3 times with the word `"incredible"`:

- start  = incredible
- first  = incre(incredible)dible
- second = increin(incredible)credibledible
- third  = increinincr(incredible)ediblecredibledible
- The final nest is increinincrincredibleediblecredibledible (depth = 3)

Valid word nests can always be collapsed to show the starting word, by reversing the process above:
```python
word = "incredible"
nest = "increinincrincredibleediblecredibledible"
```
Steps:
```python
=> "increinincrincredibleediblecredibledible" # starting nest
=> "increinincr(incredible)ediblecredibledible" # find word in nest
=> "increinincr            ediblecredibledible" # remove word
=> "increinincrediblecredibledible" # join remaining halves
=> "increin(incredible)credibledible" # find word in nest...

... repeat steps until single word remains
=> "incredible" (return True as "incredible" = word)
```
When invalid word nests are collapsed, the starting word isn't found:
```python
word = "spring"
nest = "sprspspspringringringg"
```
Steps:
```python
=> "sprspspspringringringg" # starting nest
=> "sprspsp(spring)ringringg" # find word in nest
=> "sprspsp        ringringg" # remove word
=> "sprspspringringg" # join remaining halves
=> "sprsp(spring)ringg" # find word in nest...

... repeat steps until single word remains

=> "sprg" (return False as "sprig" != "spring")
```
Given a starting word and a final word nest, return `True` if the word nest is valid. Return `False` otherwise.

## Examples
```python
valid_word_nest("deep", "deep") ➞ True

valid_word_nest("novel", "nonnonovnovnovelelelvelovelvel") ➞ True

valid_word_nest("painter", "ppaintppapaipainterinternteraintererainter") ➞ False
# Doesn't show starting word after being collapsed.

valid_word_nest("shape", "sssshapeshapehahapehpeape") ➞ False
# Word placed outside, not inside itself.
```
## Notes

- Valid word nests can only be created by repeatedly placing the word inside itself, so at any point when collapsing the nest, there should only be one instance of the word to be found.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def valid_word_nest(word: str, nest: str) -> bool:
    return False  # Put your code here!!!


test(818, valid_word_nest)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "diagram",
            "diargdiadidiadiagramgramagramgramam"
        ],
        "return": false
    },
    {
        "args": [
            "pioneer",
            "pionpippipioppionpiopipioneeroneerneereerioneerneeroneerioneeroneereer"
        ],
        "return": true
    },
    {
        "args": [
            "redeem",
            "rederedredrredredrerrrederedeememedeemedeemedeeemeemmedeemeemeemem"
        ],
        "return": false
    },
    {
        "args": [
            "feed",
            "feefeeded"
        ],
        "return": false
    },
    {
        "args": [
            "show",
            "sshssshowhowhowowhow"
        ],
        "return": true
    }
]
```

## Credits

Found on Edabit: [Word Nests (Part 2)](https://edabit.com/challenge/ZwmfET5azpvBTWoQT)
