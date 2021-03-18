# Challenge 205 - Majority Vote

Create a function that returns the majority vote in a list. A majority vote is an element that occurs `> N/2` times in a list (where `N` is the length of the list).

## Examples
```python
majority_vote(["A", "A", "B"]) ➞ "A"

majority_vote(["A", "A", "A", "B", "C", "A"]) ➞ "A"

majority_vote(["A", "B", "B", "A", "C", "C"]) ➞ None
```
## Notes

- The frequency of the majority element *must* be strictly greater than `1/2`.
- If there is no majority element, return `None`.
- If the list is empty, return `None`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Optional
import unittest


def majority_vote(votes: list[str]) -> Optional[str]:
    return  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(majority_vote(["A", "B", "B", "B", "A", "A"]), None)

    def test_2(self):
        self.assertEqual(majority_vote(["B", "B", "B"]), "B")

    def test_3(self):
        self.assertEqual(majority_vote(["A", "B", "B"]), "B")

    def test_4(self):
        self.assertEqual(majority_vote(["A", "A", "B"]), "A")

    def test_5(self):
        self.assertEqual(majority_vote(["A", "A", "A", "B", "C", "A"]), "A")

    def test_6(self):
        self.assertEqual(majority_vote(["B", "A", "B", "B", "C", "A", "B", "B"]), "B")

    def test_7(self):
        self.assertEqual(majority_vote(["A", "B", "B", "A", "C", "C"]), None)

    def test_8(self):
        self.assertEqual(majority_vote(["A", "B"]), None)

    def test_9(self):
        self.assertEqual(majority_vote(["A"]), "A")

    def test_10(self):
        self.assertEqual(majority_vote([]), None)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Majority Vote](https://edabit.com/challenge/pQavNkBbdmvSMmx5x)
