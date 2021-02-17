# Challenge 185 - Algebra Sequence

Create a function that takes a number (steps) as an argument and returns the total in that step of the sequence.

- `Step 0:` Start with 0
- `Step 1:` Add 3
- `Step 2:` Subtract 1
- *Repeat Step 1 & 2*

## Examples
```python
sequence(0) ➞ 0

sequence(1) ➞ 3

sequence(2) ➞ 2
```
## Notes

- Step (the input) is always a positive integer (or zero).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
import unittest


def sequence(steps: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sequence(5), 7)

    def test_2(self):
        self.assertEqual(sequence(0), 0)

    def test_3(self):
        self.assertEqual(sequence(6), 6)

    def test_4(self):
        self.assertEqual(sequence(99), 101)

    def test_5(self):
        self.assertEqual(sequence(2), 2)

    def test_6(self):
        self.assertEqual(sequence(1), 3)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Wash Your Hands :)](https://edabit.com/challenge/7RPtGySfZLkEHB8ac)
