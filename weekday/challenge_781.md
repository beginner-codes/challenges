# Challenge 781 - Frequency Sort

Create a function that is given a string. Sort the characters of the string and return a new string.

Sorting rules:

- Most frequent (case-sensitive) move to the front
- For the same frequency upper case characters move to the front
- For the same frequency and case sort them alphabetically.

## Examples
```python
frequency_sort("tree") ➞ "eert"

frequency_sort("cccaaa") ➞ "aaaccc"

frequency_sort("Aabb") ➞ "bbAa"
```
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


def frequency_sort(string: str) -> str:
    return ""  # Put your code here!!!


test(781, frequency_sort)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "tree"
        ],
        "return": "eert"
    },
    {
        "args": [
            "cjjNxDdztEepNNjcpdevqpDqNxcpEzDhJxnxDpuJqJPdppxzddduiojuthJuhDNvPhcdteudPqDocUdizexzhczhzdezdqcJpJiJNeuDuNDEjcqtnhncDqqjztEztEdnDJiutjjiJsiopDDjnidEiujpxecxOcxtOxcpPnipdncjJeidPpuvjhzktUtvdDnuDxpjPitjNhPdiicivDxPPhttthxpuJdxOJxspxkhD"
        ],
        "return": "ddddddddddddddddddDDDDDDDDDDDDDDDDppppppppppppppppxxxxxxxxxxxxxxxxcccccccccccccciiiiiiiiiiiiiijjjjjjjjjjjjjjttttttttttttttJJJJJJJJJJJJhhhhhhhhhhhhuuuuuuuuuuuuzzzzzzzzzzzPPPPPPPPPNNNNNNNNeeeeeeeennnnnnnnqqqqqqqqEEEEEEvvvvvOOOoooUUkkss"
    },
    {
        "args": [
            "cccaaa"
        ],
        "return": "aaaccc"
    },
    {
        "args": [
            "Aabb"
        ],
        "return": "bbAa"
    },
    {
        "args": [
            "qqXQwlbYOboaooqXixQqQqiOBixaxQqQxbQaBqqyQhBQQwqOQqXX"
        ],
        "return": "QQQQQQQQQQqqqqqqqqqqXXXXxxxxBBBOOOaaabbbiiiooowwYhly"
    }
]
```

## Credits

Found on Edabit: [Sort Characters by Frequency, Case, Alphabet](https://edabit.com/challenge/ik9CtowAndmAiStze)
