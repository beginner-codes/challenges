# Challenge 451 - The Most Brilliant Exciting Fantastic Number

Given a number, return a sentence which describes the number in the following ways.

- Always start the string with "The most".
- If `n` is evenly divisible by `1`, add `"brilliant"` to the sentence.
- If `n` is evenly divisible by `2`, add `"exciting"` to the sentence.
- ... 3, add `"fantastic"` to the sentence.
- ... 4, add `"virtuous"` to the sentence.
- ... 5, add `"heart-warming"` ...
- ... 6, add `"tear-jerking"` ...
- ... 7, add `"beautiful"` ...
- ... 8, add `"exhilarating"` ...
- ... 9, add `"emotional"` ...
- If `n` is evenly divisible by `10`, add inspiring to the sentence.
- Always end the string with `"number is n!"`

## Examples
```python
describe_num(13) ➞ "The most brilliant number is 13!"
# 13 is evenly divisble by 1 only

describe_num(4) ➞ "The most brilliant exciting virtuous number is 4!"
# 4 is evenly divisible by 1, 2 and 4

describe_num(21) ➞ "The most brilliant fantastic beautiful number is 21!"
# 21 is evenly divisible by 1, 3 and 7

describe_num(60) ➞ "The most brilliant exciting fantastic virtuous heart-warming tear-jerking inspiring number is 60!"
# 60 is evenly divisible by 1, 2, 3, 4, 5, 6 and 10
```
## Notes

- Add words to the sentence in the order going down the list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
  {
      "args": [13],
      "return": "The most brilliant number is 13!"
  },
  {
    "args": [4],
    "return": "The most brilliant exciting virtuous number is 4!"
  },
  {
    "args": [21],
    "return": "The most brilliant fantastic beautiful number is 21!"
  },
  {
    "args": [60],
    "return": "The most brilliant exciting fantastic virtuous heart-warming tear-jerking inspiring number is 60!"
  },
  {
    "args": [56],
    "return": "The most brilliant exciting virtuous beautiful exhilarating number is 56!"
  },
  {
    "args": [47],
    "return": "The most brilliant number is 47!"
  },
  {
    "args": [11],
    "return":  "The most brilliant heart-warming number is 115!"
  },
  {
    "args": [30],
    "return":  "The most brilliant exciting fantastic virtuous heart-warming tear-jerking inspiring number is 300!"
  },
  {
    "args": [20],
    "return":  "The most brilliant fantastic number is 201!"
  },
  {
    "args": [22],
    "return":  "The most brilliant exciting virtuous beautiful exhilarating number is 224!"
  }
]
```
## Credits

Found on Edabit: [The Most Brilliant Exciting Fantastic Number!](https://edabit.com/challenge/3JX75W5Xvun63RH9H)
