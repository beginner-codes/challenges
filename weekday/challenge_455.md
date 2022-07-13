# Challenge 455 - Find First Character That Repeats

Create a function that takes a string and returns the first character that repeats. If there is no repeat of a character, then return `"-1"`.

## Examples
```python
first_repeat("legolas") ➞ "l"

first_repeat("Gandalf") ➞ "a"

first_repeat("Balrog") ➞ "-1"

first_repeat("Isildur") ➞ "-1"
```
## Notes

- Tests are case-sensitive.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
    {
        "args": [
            "legolas"
        ],
        "return": "l"
    },
    {
        "args": [
            "Balrog"
        ],
        "return": "-1"
    },
    {
        "args": [
            "Isildur"
        ],
        "return": "-1"
    },
    {
        "args": [
            "Gollum"
        ],
        "return": "l"
    },
    {
        "args": [
            "Galadriel"
        ],
        "return": "a"
    },
    {
        "args": [
            "pippin"
        ],
        "return": "p"
    },
    {
        "args": [
            "Saruman"
        ],
        "return": "a"
    }
]
```
## Credits

Found on Edabit: [Find First Character That Repeats](https://edabit.com/challenge/SdGE4ZBtuMKyxDqQ6)
