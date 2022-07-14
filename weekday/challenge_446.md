# Challenge 446 - Abbreviations Unique?

You are given two inputs:

- An array of abbreviations.
- An array of words.

Write a function that returns `True` if each abbreviation uniquely identifies a word, and `False` otherwise.

## Examples
```python
unique_abbrev(["ho", "h", "ha"], ["house", "hope", "happy"]) ➞ False
# "ho" and "h" are ambiguous and can identify either "house" or "hope"

unique_abbrev(["s", "t", "v"], ["stamina", "television", "vindaloo"]) ➞ True

unique_abbrev(["bi", "ba", "bat"], ["big", "bard", "battery"]) ➞ False

unique_abbrev(["mo", "ma", "me"], ["moment", "many", "mean"]) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
  {
    "args": [
      ["s", "t", "v"],
      ["stamina", "television", "vindaloo"]
    ],
    "return": true
  },
  {
    "args": [
      ["mo", "ma", "me"],
      ["moment", "many", "mean"]
    ],
    "return": true
  },
  {
    "args": [
      ["at", "o", "abe"],
      ["atom", "original", "abet"]
    ],
    "return": true
  },
  {
    "args": [
      ["rh", "par", "re"],
      ["rhino", "parry", "residue"]
    ],
    "return": true
  },
  {
    "args": [
      ["ho", "h", "ha"],
      ["house", "hope", "happy"]
    ],
    "return": false
  }
]

```
## Credits

Found on Edabit: [Abbreviations Unique?](https://edabit.com/challenge/tjMNAEgkNvM5eyEqJ)
