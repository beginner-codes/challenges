# Challenge 240 - Stupid Addition

Create a function that takes two parameters and, if both parameters are strings, add them as if they were integers or if the two parameters are integers, concatenate them.

## Examples
```python
stupid_addition(1, 2) ➞ "12"

stupid_addition("1", "2") ➞ 3

stupid_addition("1", 2) ➞ None
```
## Notes

- If the two parameters are different data types, return `None`.
- All parameters will either be strings or integers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from typing import Union
import unittest


def stupid_addition(
    first_number: Union[int, str], second_number: Union[int, str]
) -> Union[int, str]:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(stupid_addition(1, 2), "12")

    def test_2(self):
        self.assertEqual(stupid_addition("1", "2"), 3)

    def test_3(self):
        self.assertEqual(stupid_addition(1, "2"), None)

    def test_4(self):
        self.assertEqual(stupid_addition("1", 2), None)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Stupid Addition](https://edabit.com/challenge/6dnhESWBcTMMF3gsa)
