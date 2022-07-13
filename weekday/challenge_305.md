# Challenge 305 - Ones, Threes and Nines

Given a number, figure out how many ones, threes and nines you could fit into that number. You must create a class that your function will return an instance of. The class should have attributes (`self.ones`, `self.threes`, `self.nines`) to do this.

## Examples
```python
n1 = ones_threes_nines(5)
n1.nines ➞ 0

n1.ones ➞ 5

n1.threes ➞ 1
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from typing import Protocol
import unittest


class OnesThreesNinesProtocol(Protocol):
    ones: int
    threes: int
    nines: int


def ones_threes_nines(n: int) -> OnesThreesNinesProtocol:
    return OnesThreesNinesProtocol()  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(ones_threes_nines(0).ones, 0)

    def test_2(self):
        self.assertEqual(ones_threes_nines(1).threes, 0)

    def test_3(self):
        self.assertEqual(ones_threes_nines(2).nines, 0)

    def test_4(self):
        self.assertEqual(ones_threes_nines(3).ones, 3)

    def test_5(self):
        self.assertEqual(ones_threes_nines(4).threes, 1)

    def test_6(self):
        self.assertEqual(ones_threes_nines(10).nines, 1)

    def test_7(self):
        self.assertEqual(ones_threes_nines(13).ones, 13)

    def test_8(self):
        self.assertEqual(ones_threes_nines(15).threes, 5)

    def test_9(self):
        self.assertEqual(ones_threes_nines(17).nines, 1)

    def test_10(self):
        self.assertEqual(ones_threes_nines(20).nines, 2)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Ones, Threes and Nines (Version #1)](https://edabit.com/challenge/X6xZ2EaqqQbGF7Bwv)
