# Challenge 210 - Hashtag Generator

Create a function that is a Hashtag Generator by using the following rules:

- The output must start with a hashtag (#).
- Each word in the string must have its first letter capitalized.
- If the final result, a single string, is longer than 140 characters, the function should return `False`.
- If either the input (str) or the result is an empty string, the function should return `False`.

## Examples
```python
generate_hashtag("    Hello     World   " ) ➞ "#HelloWorld"

generate_hashtag("") ➞ false
# Expected an empty string to return false

generate_hashtag("Edabit Is Great") ➞ "#EdabitIsGreat"
# Should remove spaces.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from typing import Union
import unittest


def generate_hashtag(phrase: str) -> Union[str, bool]:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(generate_hashtag(""), False)

    def test_2(self):
        self.assertEqual(generate_hashtag(" " * 100), False)

    def test_3(self):
        self.assertEqual(
            generate_hashtag("Do We have A Hashtag"),
            "#DoWeHaveAHashtag",
        )

    def test_4(self):
        self.assertEqual(generate_hashtag("beginner py"), "#BeginnerPy")

    def test_5(self):
        self.assertEqual(
            generate_hashtag("Beginner Py Is Great"),
            "#BeginnerPyIsGreat",
        )

    def test_6(self):
        self.assertEqual(
            generate_hashtag("beginner py is great"),
            "#BeginnerPyIsGreat",
        )

    def test_7(self):
        self.assertEqual(generate_hashtag("beginner" + " " * 140 + "py"), "#BeginnerPy")

    def test_8(self):
        self.assertEqual(
            generate_hashtag(
                "Smmmmmmmmmmmmmmmmmmmmmmmmmmmmaaaaaaaaaaaaaaaaaaaaaaaaaaaaallllllllllllllllllllllllllllllllllllllllllll"
                "lllllllllllllllllllllllllllllllllllll Dog"
            ),
            False,
        )

    def test_9(self):
        self.assertEqual(generate_hashtag("e" * 121), "#E" + "e" * 120)

    def test_10(self):
        self.assertEqual(generate_hashtag("e" * 140), False)

    def test_11(self):
        self.assertEqual(generate_hashtag("    Hello     World   "), "#HelloWorld")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Hashtag Generator](https://edabit.com/challenge/RvCEzuqacuBA94ZfP)
