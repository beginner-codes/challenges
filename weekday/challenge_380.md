# Challenge 380 - Find the True Equations

In this challenge you will be given a list containing equations, with each equation written as a string. Here's an example:
```python
["1+1=2", "2+2=3", "5*5=10", "3/3=1"]
```
If you do the math, you'll see that the equations `"1+1=2"` and `"3/3=1"` are actually true while `"2+2=3"` and `"5*5=10"` are false nonsense.

Write a function which, given a list of equations as above, returns only the true equations. For instance, for the example above the output should be:
```python
["1+1=2", "3/3=1"]
```
## Examples
```python
true_equations(["2*2=4"]) ➞ ["2*2=4"]

true_equations(["1+1=3", "3-1=1"]) ➞ []

true_equations(["1+1=2", "2+2=3", "5*5=10", "3/3=1"]) ➞ ["1+1=2", "3/3=1"]
```
## Notes

- If all equations are false, return the empty list `[]`, as in the second example.
- The equations will only involve the elementary operations: `+`, `-`, `*`, `/`

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def true_equations(equations: list[str]) -> list[str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(true_equations(["2*2=4"]), ["2*2=4"])

    def test_2(self):
        self.assertListEqual(true_equations(["1+1=3", "3-1=1"]), [])

    def test_3(self):
        self.assertListEqual(
            true_equations(["1+1=2", "2+2=3", "5*5=10", "3/3=1"]), ["1+1=2", "3/3=1"]
        )

    def test_4(self):
        self.assertListEqual(
            true_equations(["4/2=2", "8-4=2", "5*5=25", "3/3=14"]), ["4/2=2", "5*5=25"]
        )

    def test_5(self):
        self.assertListEqual(
            true_equations(["1-1=0", "2/2=1", "13+9=22", "1*9=9"]),
            ["1-1=0", "2/2=1", "13+9=22", "1*9=9"],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Find the True Equations](https://edabit.com/challenge/RcauxLL2SqHYpzZrz)
