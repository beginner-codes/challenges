# Challenge 379 - Power of Two

Write a function that returns `True` if an integer can be expressed as a power of base value 2 and `False` otherwise.

## Examples
```python
power_of_two(32) ➞ True

power_of_two(1) ➞ True

power_of_two(18) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def power_of_two(number: int) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(power_of_two(32))

    def test_2(self):
        self.assertTrue(power_of_two(1))

    def test_3(self):
        self.assertFalse(power_of_two(18))

    def test_4(self):
        self.assertFalse(power_of_two(329))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Power of Two](https://edabit.com/challenge/mz7mpEnMByAvBzMrc)
