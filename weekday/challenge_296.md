# Challenge 296 - International Greetings

Suppose you have a guest list of students and the country they are from, stored as key-value pairs in a dictionary.
```
GUEST_LIST = {
    "Randy": "Germany",
    "Karla": "France",
    "Wendy": "Japan",
    "Norman": "England",
    "Sam": "Argentina"
}
```
Write a function that takes in a name and returns a name tag, that should read:
```
"Hi! I'm [name], and I'm from [country]."
```
If the name is not in the dictionary, return:
```
"Hi! I'm a guest."
```
## Examples
```python
greeting("Randy") ➞ "Hi! I'm Randy, and I'm from Germany."

greeting("Sam") ➞ "Hi! I'm Sam, and I'm from Argentina."

greeting("Monti") ➞ "Hi! I'm a guest."
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Union
import unittest


def fizz_buzz(maximum: int) -> list[Union[int, str]]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(fizz_buzz(10), [1, 2, 'Fizz', 4, 'Buzz', 'Fizz', 7, 8, 'Fizz', 'Buzz'])

    def test_2(self):
        self.assertListEqual(
            fizz_buzz(15),
            [1, 2, 'Fizz', 4, 'Buzz', 'Fizz', 7, 8, 'Fizz', 'Buzz', 11, 'Fizz', 13, 14, 'FizzBuzz']
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [International Greetings](https://edabit.com/challenge/vAS4Hp4wzSEnQs3tZ)
