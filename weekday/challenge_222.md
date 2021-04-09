# Challenge 221 - A Long Long Time

Create a function that returns the simplified version of a fraction.

## Examples
```python
simplify("4/6") ➞ "2/3"

simplify("10/11") ➞ "10/11"

simplify("100/400") ➞ "1/4"

simplify("8/4") ➞ "2"
```
## Notes

- A fraction is simplified if there are no common factors (except 1) between the numerator and the denominator. For example, `4/6` is not simplified, since `4` and `6` both share `2` as a factor.
- If improper fractions can be transformed into integers, do so in your code

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def simplify(fraction: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(simplify("5/7"), "5/7")

    def test_2(self):
        self.assertEqual(simplify("4/6"), "2/3")

    def test_3(self):
        self.assertEqual(simplify("11/10"), "11/10")

    def test_4(self):
        self.assertEqual(simplify("8/4"), "2")

    def test_5(self):
        self.assertEqual(simplify("7/4"), "7/4")

    def test_6(self):
        self.assertEqual(simplify("6/4"), "3/2")

    def test_7(self):
        self.assertEqual(simplify("300/200"), "3/2")

    def test_8(self):
        self.assertEqual(simplify("50/25"), "2")

    def test_9(self):
        self.assertEqual(simplify("5/45"), "1/9")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Simplified Fractions](https://edabit.com/challenge/vQgmyjcjMoMu9YGGW)
