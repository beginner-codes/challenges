# Challenge 737 - Bird Names to Four Letter Bird Codes

In the world of birding there are four-letter codes for the common names of birds. These codes are created by some
simple rules:

- If the bird's name has only one word, the code takes the first four letters of that word.
- If the name is made up of two words, the code takes the first two letters of each word.
- If the name is made up of three words, the code is created by taking the first letter from the first two words and the
  first two letters from the third word.
- If the name is four words long, the code uses the first letter from all the words.

There are other ways codes are created, but this challenge will only use the four rules listed above.

In this challenge you will write a function that takes a list of strings of common bird names and create the codes for
those names based on the rules above. The function will return a list of codes in the same order in which the input
names were presented.

## Examples

```python
bird_code(["Black-Capped Chickadee", "Common Tern"]) ➞ ["BCCH", "COTE"]

bird_code(["American Redstart", "Northern Cardinal"]) ➞ ["AMRE", "NOCA"]

bird_code(["Bobolink", "American White Pelican"]) ➞ ["BOBO", "AWPE"]
```

## Notes

- The four-letter codes in the returned list should be in UPPER CASE.
- If a common name has a hyphen/dash, it should be considered a space.

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


def bird_code(birds: list[str]) -> list[str]:
    return []  # Put your code here!!!


test(737, bird_code)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      [
        "Black-Crowned Night Heron",
        "Northern Mockingbird",
        "Eastern Meadowlark",
        "Dark-Eyed Junco",
        "Red-Bellied Woodpecker"
      ]
    ],
    "return": [
      "BCNH",
      "NOMO",
      "EAME",
      "DEJU",
      "RBWO"
    ]
  },
  {
    "args": [
      [
        "Fox Sparrow",
        "White-Winged Crossbill",
        "Veery",
        "American Coot",
        "Sora",
        "Northern Rough-Winged Swallow",
        "Purple Martin"
      ]
    ],
    "return": [
      "FOSP",
      "WWCR",
      "VEER",
      "AMCO",
      "SORA",
      "NRWS",
      "PUMA"
    ]
  },
  {
    "args": [
      [
        "American Redstart",
        "Northern Cardinal",
        "Pine Grosbeak",
        "Barred Owl",
        "Starling",
        "Cooper's Hawk",
        "Pigeon"
      ]
    ],
    "return": [
      "AMRE",
      "NOCA",
      "PIGR",
      "BAOW",
      "STAR",
      "COHA",
      "PIGE"
    ]
  },
  {
    "args": [
      [
        "Common Tern",
        "Black-Capped Chickadee"
      ]
    ],
    "return": [
      "COTE",
      "BCCH"
    ]
  },
  {
    "args": [
      [
        "Great Crested Flycatcher",
        "Bobolink",
        "American White Pelican",
        "Red-Tailed Hawk",
        "Eastern Screech Owl",
        "Blue Jay"
      ]
    ],
    "return": [
      "GCFL",
      "BOBO",
      "AWPE",
      "RTHA",
      "ESOW",
      "BLJA"
    ]
  },
  {
    "args": [
      [
        "Scarlet Tanager",
        "Great Blue Heron",
        "Eastern Phoebe",
        "American Black Duck",
        "Mallard",
        "Canvasback",
        "Merlin",
        "Ovenbird"
      ]
    ],
    "return": [
      "SCTA",
      "GBHE",
      "EAPH",
      "ABDU",
      "MALL",
      "CANV",
      "MERL",
      "OVEN"
    ]
  }
]
```

## Credits

Found on Edabit: [Bird Names to Four Letter Bird Codes](https://edabit.com/challenge/hpJsoWBBHWKZ9NcAi)
