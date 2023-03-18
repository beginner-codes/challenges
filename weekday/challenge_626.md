# Challenge 626 - Cleaning Project Files

You are in the midst of organizing all of your coding projects. It's a mess! Every file you've ever created is located in the same folder.

To clean it up, you've decided that you will use one of two organization methods.

- The prefix method: You will group all files with the same project name under the same folder.
- The suffix method: You will group all files with the same extension under the same folder.

Create a function that takes in the current folder sorts the files according to the organization method (prefix or suffix). A folder is a grouping of files in the same list.

## Examples
```python
# Sorting by project name (ex1 and ex2)
clean_up(["ex1.html", "ex1.js", "ex2.html", "ex2.js"], "prefix") ➞ [
  ["ex1.html", "ex1.js"],
  ["ex2.html", "ex2.js"]
]

# Sorting by extension (.html and .js)
clean_up(["ex1.html", "ex1.js", "ex2.html", "ex2.js"], "suffix") ➞ [
  ["ex1.html", "ex2.html"],
  ["ex1.js", "ex2.js"]
]

clean_up(["music_app.js", "music_app.png", "music_app.wav", "tetris.png", "tetris.js"], "prefix") ➞ [
  ["music_app.js", "music_app.png", "music_app.wav"],
  ["tetris.png", "tetris.js"]
]

clean_up(["_1.rb", "_2.rb", "_3.rb", "_4.rb"], "suffix") ➞ [
  ["_1.rb", "_2.rb", "_3.rb", "_4.rb"]
]

clean_up(["_1.rb", "_2.rb", "_3.rb", "_4.rb"], "prefix") ➞ [
  ["_1.rb"], ["_2.rb"],
  ["_3.rb"], ["_4.rb"]
]
```
## Notes

- Keep elements in the same relative order.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def clean_up(files: list[str], method: str) -> list[list[str]]:
    return []  # Put your code here!!!


test(626, clean_up)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "_1.rb",
                "_2.rb",
                "_3.rb",
                "_4.rb"
            ],
            "prefix"
        ],
        "return": [
            [
                "_1.rb"
            ],
            [
                "_2.rb"
            ],
            [
                "_3.rb"
            ],
            [
                "_4.rb"
            ]
        ]
    },
    {
        "args": [
            [
                "project1.html",
                "project2.html",
                "project1.css",
                "project2.css",
                "project1.js",
                "project2.js"
            ],
            "suffix"
        ],
        "return": [
            [
                "project1.html",
                "project2.html"
            ],
            [
                "project1.css",
                "project2.css"
            ],
            [
                "project1.js",
                "project2.js"
            ]
        ]
    },
    {
        "args": [
            [
                "_1.rb",
                "_2.rb",
                "_3.rb",
                "_4.rb"
            ],
            "suffix"
        ],
        "return": [
            [
                "_1.rb",
                "_2.rb",
                "_3.rb",
                "_4.rb"
            ]
        ]
    },
    {
        "args": [
            [
                "music_app.js",
                "music_app.png",
                "music_app.wav",
                "tetris.png",
                "tetris.js"
            ],
            "prefix"
        ],
        "return": [
            [
                "music_app.js",
                "music_app.png",
                "music_app.wav"
            ],
            [
                "tetris.png",
                "tetris.js"
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Cleaning Project Files](https://edabit.com/challenge/NC888jKPkquSDqaaH)
