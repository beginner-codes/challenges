# Challenge 678 - Extract Tweet Mentions

Your job is to make a function that searches tweets for user and hashtag mentions. Only return the @ and # handles.

## Examples
```python
extract_mentions("Visit us at @beginnercodes") ➞ "@beginnercodes"

extract_mentions("Follow @JavaScript") ➞ "@JavaScript"

extract_mentions("#Honesty is the best @policy!!") ➞ "#Honesty @policy"
```
## Notes

- Make sure the function doesn't return `.` `,` `!` or `?`

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def extract_mentions(tweet: str) -> str:
    return ""  # Put your code here!!!


test(678, extract_mentions)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "#Finally, a test!"
        ],
        "return": "#Finally"
    },
    {
        "args": [
            "Follow @JavaScript"
        ],
        "return": "@JavaScript"
    },
    {
        "args": [
            "The @committee consists of #eminent #jurists."
        ],
        "return": "@committee #eminent #jurists"
    },
    {
        "args": [
            "@RonaldRoss was awarded the Nobel Prize for his work on the transmission of #malaria."
        ],
        "return": "@RonaldRoss #malaria"
    },
    {
        "args": [
            "Visit us at @beginnercodes"
        ],
        "return": "@beginnercodes"
    }
]
```
## Credits

Found on Edabit: [Twitter Link Finder](https://edabit.com/challenge/AqcGgqbMFhSqn44Qx)
