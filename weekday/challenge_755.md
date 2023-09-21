# Challenge 755 - Sentence Searcher

Create a function that returns the whole of the first sentence which contains a specific word. Include the full stop at the end of the sentence.

## Examples
```python
txt = "I have a cat. I have a mat. Things are going swell."

sentence_searcher(txt, "have") ➞ "I have a cat."

sentence_searcher(txt, "MAT") ➞ "I have a mat."

sentence_searcher(txt, "things") ➞ "Things are going swell."

sentence_searcher(txt, "flat") ➞ ""
```
## Notes

- Sentences will always end with a period.
- Your function should not be case-sensitive.
- Return an empty string if the word isn't found in the sentence.

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


def sentence_searcher(sentence: str, word: str) -> str:
    return ""  # Put your code here!!!


test(755, sentence_searcher)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "I have a cat. I have a mat. Things are going swell.",
            "flat"
        ],
        "return": ""
    },
    {
        "args": [
            "I have a cat. I have a mat. Things are going swell.",
            "cat"
        ],
        "return": "I have a cat."
    },
    {
        "args": [
            "I have a cat. I have a mat. Things are going swell.",
            "things"
        ],
        "return": "Things are going swell."
    },
    {
        "args": [
            "I have a cat. I have a mat. Things are going swell.",
            "MAT"
        ],
        "return": "I have a mat."
    },
    {
        "args": [
            "I have a cat. I have a mat. Things are going swell.",
            "swell"
        ],
        "return": "Things are going swell."
    },
    {
        "args": [
            "I have a cat. I have a mat. Things are going swell.",
            "Have"
        ],
        "return": "I have a cat."
    }
]
```

## Credits

Found on Edabit: [Sentence Searcher](https://edabit.com/challenge/Q72X3J8jq7SzSSXui)
