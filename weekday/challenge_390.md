# Challenge 390 - Simplified Josephus

Given a group of people, find the survivor. Starting from the first person, they kill the person to their left and the next surviving person kills the person to their left. This keeps happening until 1 person survives. Return that person's number.

## Examples
```python
josephus(1) ➞ 1

josephus(8) ➞ 1

josephus(41) ➞ 19
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def josephus(num_people: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(josephus(1), 1)

    def test_2(self):
        self.assertEqual(josephus(41), 19)

    def test_3(self):
        self.assertEqual(josephus(8), 1)

    def test_4(self):
        self.assertEqual(josephus(5), 3)

    def test_5(self):
        self.assertEqual(josephus(7), 7)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Simplified Josephus](https://edabit.com/challenge/L9Zh7dWsENnE9P6qc)
