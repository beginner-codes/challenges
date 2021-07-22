# Challenge 295 - Fizz Buzz

Create a function that returns a list of all the numbers from 1 to an integer argument. For multiples of three use `“Fizz”` instead of the number and for the multiples of five use `“Buzz”`. For numbers which are multiples of both three and five use `“FizzBuzz”`.

## Example
```python
fizz_buzz(10) ➞ [1, 2, "Fizz", 4, "Buzz", "Fizz", 7, 8, "Fizz", "Buzz"]

fizz_buzz(15) ➞ [1, 2, "Fizz", 4, "Buzz", "Fizz", 7, 8, "Fizz", "Buzz", 11, "Fizz", 13, 14, "FizzBuzz"]
```
## Notes

- Make sure to return a list.

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

Found on Edabit: [The Fizz Buzz Test](https://edabit.com/challenge/646cCaFig6AP89YRo)
