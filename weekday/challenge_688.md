# Challenge 688 - AlTeRnAtInG cApS 

Create a function that alternates the case of the letters in a string (known as Spongecase).

## Examples
```python
alternating_caps("Hello") ➞ "HeLlO"

alternating_caps("How are you?") ➞ "HoW aRe YoU?"

alternating_caps("OMG this website is awesome!") ➞ "OmG tHiS wEbSiTe Is AwEsOmE!"
```
## Notes

- The first letter should always be UPPERCASE.
- Ignore spaces.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def alternating_caps(string: str) -> str:
    return ""  # Put your code here!!!


test(688, alternating_caps)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "alternating caps"
        ],
        "return": "AlTeRnAtInG cApS"
    },
    {
        "args": [
            "The quick brown fox jumps over the lazy dog"
        ],
        "return": "ThE qUiCk BrOwN fOx JuMpS oVeR tHe LaZy DoG"
    },
    {
        "args": [
            "What is your name?"
        ],
        "return": "WhAt Is YoUr NaMe?"
    },
    {
        "args": [
            "The intent is to provide players with a sense of pride and accomplishment for unlocking different heroes."
        ],
        "return": "ThE iNtEnT iS tO pRoViDe PlAyErS wItH a SeNsE oF pRiDe AnD aCcOmPlIsHmEnT fOr UnLoCkInG dIfFeReNt HeRoEs."
    },
    {
        "args": [
            "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        ],
        "return": "LoReM iPsUm DoLoR sIt AmEt CoNsEcTeTuR aDiPiSiCiNg ElIt."
    },
    {
        "args": [
            "OMG this website is awesome!"
        ],
        "return": "OmG tHiS wEbSiTe Is AwEsOmE!"
    }
]
```
## Credits

Found on Edabit: [AlTeRnAtInG cApS](https://edabit.com/challenge/hzs9hZXpgYdGM3iwB)
