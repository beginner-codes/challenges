# Challenge 762 - Word Buckets

Write a function that divides a phrase into word buckets, with each bucket containing `n` or fewer characters. Only include full words inside each bucket.

## Examples
```python
split_into_buckets("she sells sea shells by the sea", 10)
➞ ["she sells", "sea shells", "by the sea"]

split_into_buckets("the mouse jumped over the cheese", 7)
➞ ["the", "mouse", "jumped", "over", "the", "cheese"]

split_into_buckets("fairy dust coated the air", 20)
➞ ["fairy dust coated", "the air"]

split_into_buckets("a b c d e", 2)
➞ ["a", "b", "c", "d", "e"]
```
## Notes

- Spaces count as one character.
- Trim beginning and end spaces for each word bucket.
- If buckets are too small to hold a single word, return an empty list: []
- The final goal isn't to return just the words with a length equal (or lower) to the given `n`, but to return the entire phrase bucketized (if possible).

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


def split_into_buckets(phrase: str, bucket_size: int) -> list[str]:
    return []  # Put your code here!!!


test(762, split_into_buckets)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "rich magnificent trees dotted the landscape",
            18
        ],
        "return": [
            "rich magnificent",
            "trees dotted the",
            "landscape"
        ]
    },
    {
        "args": [
            "a b c d e",
            2
        ],
        "return": [
            "a",
            "b",
            "c",
            "d",
            "e"
        ]
    },
    {
        "args": [
            "a b c d e",
            3
        ],
        "return": [
            "a b",
            "c d",
            "e"
        ]
    },
    {
        "args": [
            "beep bo bee bop bee bo bo bop",
            6
        ],
        "return": [
            "beep",
            "bo bee",
            "bop",
            "bee bo",
            "bo bop"
        ]
    },
    {
        "args": [
            "rich magnificent trees dotted the landscape",
            22
        ],
        "return": [
            "rich magnificent trees",
            "dotted the landscape"
        ]
    }
]
```

## Credits

Found on Edabit: [Word Buckets](https://edabit.com/challenge/fbqmyDjCigbYhWLJa)
