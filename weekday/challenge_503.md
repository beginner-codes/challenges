# Challenge 503 - Wiggled Strings

Create a function that returns a list of the given string but offset by spaces. Here are some more precise instructions:

- Keep adding spaces on the left until you have the same number of spaces as the word length.
- Then keep removing spaces until you reach the original word.

Below are some helpful examples!

## Examples
```python
wiggle_string("hello") ➞ [
  "hello",
  " hello",
  "  hello",
  "   hello",
  "    hello",
  "     hello"
  "    hello",
  "   hello",
  "  hello",
  " hello",
  "hello"
]

wiggle_string("Coding") ➞ [
  "Coding",
  " Coding",
  "  Coding",
  "   Coding",
  "    Coding",
  "     Coding",
  "      Coding",
  "     Coding",
  "    Coding",
  "   Coding",
  "  Coding",
  " Coding",
  "Coding"
]

wiggle_string("Wiggle Time") ➞ [
  "Wiggle Time",
  " Wiggle Time",
  "  Wiggle Time",
  "   Wiggle Time",
  "    Wiggle Time",
  "     Wiggle Time",
  "      Wiggle Time",
  "       Wiggle Time",
  "        Wiggle Time",
  "         Wiggle Time",
  "          Wiggle Time",
  "           Wiggle Time",
  "          Wiggle Time",
  "         Wiggle Time",
  "        Wiggle Time",
  "       Wiggle Time",
  "      Wiggle Time",
  "     Wiggle Time",
  "    Wiggle Time",
  "   Wiggle Time",
  "  Wiggle Time",
  " Wiggle Time",
  "Wiggle Time"
]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def wiggle_string(string: str) -> list[str]:
    return []  # Put your code here!!!


test(503, wiggle_string)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "hello",
            " hello",
            "  hello",
            "   hello",
            "    hello",
            "     hello",
            "    hello",
            "   hello",
            "  hello",
            " hello",
            "hello"
        ],
        "return": [
            "hello"
        ]
    },
    {
        "args": [
            "Coding",
            " Coding",
            "  Coding",
            "   Coding",
            "    Coding",
            "     Coding",
            "      Coding",
            "     Coding",
            "    Coding",
            "   Coding",
            "  Coding",
            " Coding",
            "Coding"
        ],
        "return": [
            "Coding"
        ]
    },
    {
        "args": [
            "Wiggle Time",
            " Wiggle Time",
            "  Wiggle Time",
            "   Wiggle Time",
            "    Wiggle Time",
            "     Wiggle Time",
            "      Wiggle Time",
            "       Wiggle Time",
            "        Wiggle Time",
            "         Wiggle Time",
            "          Wiggle Time",
            "           Wiggle Time",
            "          Wiggle Time",
            "         Wiggle Time",
            "        Wiggle Time",
            "       Wiggle Time",
            "      Wiggle Time",
            "     Wiggle Time",
            "    Wiggle Time",
            "   Wiggle Time",
            "  Wiggle Time",
            " Wiggle Time",
            "Wiggle Time"
        ],
        "return": [
            "Wiggle Time"
        ]
    },
    {
        "args": [
            "the dog",
            " the dog",
            "  the dog",
            "   the dog",
            "    the dog",
            "     the dog",
            "      the dog",
            "       the dog",
            "      the dog",
            "     the dog",
            "    the dog",
            "   the dog",
            "  the dog",
            " the dog",
            "the dog"
        ],
        "return": [
            "the dog"
        ]
    },
    {
        "args": [
            "wiggle wiggle wiggle",
            " wiggle wiggle wiggle",
            "  wiggle wiggle wiggle",
            "   wiggle wiggle wiggle",
            "    wiggle wiggle wiggle",
            "     wiggle wiggle wiggle",
            "      wiggle wiggle wiggle",
            "       wiggle wiggle wiggle",
            "        wiggle wiggle wiggle",
            "         wiggle wiggle wiggle",
            "          wiggle wiggle wiggle",
            "           wiggle wiggle wiggle",
            "            wiggle wiggle wiggle",
            "             wiggle wiggle wiggle",
            "              wiggle wiggle wiggle",
            "               wiggle wiggle wiggle",
            "                wiggle wiggle wiggle",
            "                 wiggle wiggle wiggle",
            "                  wiggle wiggle wiggle",
            "                   wiggle wiggle wiggle",
            "                    wiggle wiggle wiggle",
            "                   wiggle wiggle wiggle",
            "                  wiggle wiggle wiggle",
            "                 wiggle wiggle wiggle",
            "                wiggle wiggle wiggle",
            "               wiggle wiggle wiggle",
            "              wiggle wiggle wiggle",
            "             wiggle wiggle wiggle",
            "            wiggle wiggle wiggle",
            "           wiggle wiggle wiggle",
            "          wiggle wiggle wiggle",
            "         wiggle wiggle wiggle",
            "        wiggle wiggle wiggle",
            "       wiggle wiggle wiggle",
            "      wiggle wiggle wiggle",
            "     wiggle wiggle wiggle",
            "    wiggle wiggle wiggle",
            "   wiggle wiggle wiggle",
            "  wiggle wiggle wiggle",
            " wiggle wiggle wiggle",
            "wiggle wiggle wiggle"
        ],
        "return": [
            "wiggle wiggle wiggle"
        ]
    },
    {
        "args": [
            "Hello World!",
            " Hello World!",
            "  Hello World!",
            "   Hello World!",
            "    Hello World!",
            "     Hello World!",
            "      Hello World!",
            "       Hello World!",
            "        Hello World!",
            "         Hello World!",
            "          Hello World!",
            "           Hello World!",
            "            Hello World!",
            "           Hello World!",
            "          Hello World!",
            "         Hello World!",
            "        Hello World!",
            "       Hello World!",
            "      Hello World!",
            "     Hello World!",
            "    Hello World!",
            "   Hello World!",
            "  Hello World!",
            " Hello World!",
            "Hello World!"
        ],
        "return": [
            "Hello World!"
        ]
    },
    {
        "args": [
            "Coding is fun!",
            " Coding is fun!",
            "  Coding is fun!",
            "   Coding is fun!",
            "    Coding is fun!",
            "     Coding is fun!",
            "      Coding is fun!",
            "       Coding is fun!",
            "        Coding is fun!",
            "         Coding is fun!",
            "          Coding is fun!",
            "           Coding is fun!",
            "            Coding is fun!",
            "             Coding is fun!",
            "              Coding is fun!",
            "             Coding is fun!",
            "            Coding is fun!",
            "           Coding is fun!",
            "          Coding is fun!",
            "         Coding is fun!",
            "        Coding is fun!",
            "       Coding is fun!",
            "      Coding is fun!",
            "     Coding is fun!",
            "    Coding is fun!",
            "   Coding is fun!",
            "  Coding is fun!",
            " Coding is fun!",
            "Coding is fun!"
        ],
        "return": [
            "Coding is fun!"
        ]
    },
    {
        "args": [
            "123456789",
            " 123456789",
            "  123456789",
            "   123456789",
            "    123456789",
            "     123456789",
            "      123456789",
            "       123456789",
            "        123456789",
            "         123456789",
            "        123456789",
            "       123456789",
            "      123456789",
            "     123456789",
            "    123456789",
            "   123456789",
            "  123456789",
            " 123456789",
            "123456789"
        ],
        "return": [
            "123456789"
        ]
    },
    {
        "args": [
            "qwertyuiop",
            " qwertyuiop",
            "  qwertyuiop",
            "   qwertyuiop",
            "    qwertyuiop",
            "     qwertyuiop",
            "      qwertyuiop",
            "       qwertyuiop",
            "        qwertyuiop",
            "         qwertyuiop",
            "          qwertyuiop",
            "         qwertyuiop",
            "        qwertyuiop",
            "       qwertyuiop",
            "      qwertyuiop",
            "     qwertyuiop",
            "    qwertyuiop",
            "   qwertyuiop",
            "  qwertyuiop",
            " qwertyuiop",
            "qwertyuiop"
        ],
        "return": [
            "qwertyuiop"
        ]
    },
    {
        "args": [
            "python javascript",
            " python javascript",
            "  python javascript",
            "   python javascript",
            "    python javascript",
            "     python javascript",
            "      python javascript",
            "       python javascript",
            "        python javascript",
            "         python javascript",
            "          python javascript",
            "           python javascript",
            "            python javascript",
            "             python javascript",
            "              python javascript",
            "               python javascript",
            "                python javascript",
            "                 python javascript",
            "                python javascript",
            "               python javascript",
            "              python javascript",
            "             python javascript",
            "            python javascript",
            "           python javascript",
            "          python javascript",
            "         python javascript",
            "        python javascript",
            "       python javascript",
            "      python javascript",
            "     python javascript",
            "    python javascript",
            "   python javascript",
            "  python javascript",
            " python javascript",
            "python javascript"
        ],
        "return": [
            "python javascript"
        ]
    }
]
```
## Credits

Found on Edabit: [Wiggled Strings](https://edabit.com/challenge/xYRNzJB7kAXXEQSdF)
