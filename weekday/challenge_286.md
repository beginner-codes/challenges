# Challenge 286 - String Builder

Write a function that returns a function that will build a string. The function should take a string and return a function that takes a second string and concatenates it to the end of the first string.
 
## Example
```python
builder = string_builder("Beginner.py is the ")

builder("best") -> "Beginner.py is the best"

builder("coolest") -> "Beginner.py is the coolest" 

builder("most awesomest") -> "Beginner.py is the most awesomest" 
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from typing import Callable
import unittest


def string_builder(string: str) -> Callable[[str], str]:
    return lambda s: string + s  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        builder = string_builder("My name is ")
        for name in ["John", "Bob", "Jane", "Ann"]:
            self.assertEqual(builder(name), f"My name is {name}")

    def test_2(self):
        builder = string_builder("My cat is bigger than ")
        for than_a in ["a dog", "a donkey", "a horse", "an elephant"]:
            self.assertEqual(builder(than_a), f"My cat is bigger than {than_a}")

    def test_3(self):
        builder = string_builder("Coding is more fun than ")
        for than in [
            "counting beans",
            "jumping in puddles",
            "eating ice cream",
            "the circus",
        ]:
            self.assertEqual(builder(than), f"Coding is more fun than {than}")

    def test_4(self):
        builder = string_builder("Beginner.py is the ")

        for is_the in ["best", "coolest", "most awesomest"]:
            self.assertEqual(builder(is_the), f"Beginner.py is the {is_the}")


if __name__ == "__main__":
    unittest.main()
```
## Credits

From the brains of Zech
