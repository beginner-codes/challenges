# Challenge 256 - Square Every Digit

Create a function that squares every digit of a number.

## Examples
```python
square_digits(9119) ➞ 811181

square_digits(2483) ➞ 416649

square_digits(3212) ➞ 9414
```
## Notes

- The function receives an integer and must return an integer.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def square_digits(number: int) -> bool:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(square_digits(9119), 811181)

    def test_2(self):
        self.assertEqual(square_digits(8726), 6449436)

    def test_3(self):
        self.assertEqual(square_digits(9763), 8149369)

    def test_4(self):
        self.assertEqual(square_digits(2230), 4490)

    def test_5(self):
        self.assertEqual(square_digits(2797), 4498149)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Square Every Digit](https://edabit.com/challenge/Tnjbf6pdFsCjmaF8p)
