# Challenge 387 - Standard Deviation

The central tendency measures (mean, mode and median) sometimes aren't enough in data set analysis. For example, given two lists `A=[15, 15, 15, 14, 16]` and `B=[2, 7, 14, 22, 30]` the mean is `μ=15` in both cases, however the values of second list are clearly more spread out from the average value. The standard deviation (also called sigma, the greek lowercase letter `σ`) measures the spread of the values in a data set and transform the "clearly more spread out than" assertion in a proofed statistical assertion.

The standard deviation is calculated following five steps:

- Obtain the mean of the data set.
- For each value in the set calculate the absolute difference between the value and the mean.
- Square each value obtained and sum them cumulatively.
- Divide the result by the data set length.
- Get the square root of the value obtained.
- Given a list of values return the standard deviation rounded to the nearest hundredth.

## Examples
```python
standard_deviation([3, 5, 7]) ➞ 1.63
# |(3-5)|+|(5-5)|+|(7-5)| = 2² + 0 + 2² = 8 / 3 = square root of 2.66 = 1.63

standard_deviation([5, 5, 5]) ➞ 0
# Values aren't deviating from the mean.

standard_deviation([-3, -5, -7]) ➞ 1.63
# Remember: absolute differences!
```
## Notes

- All given lists are valid, no exceptions to handle.
- Lists can contain either positive or negative integers.
- Remember to round to the nearest hundredth at the end.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def standard_deviation(numbers: list[int]) -> float:
    return float("NaN")  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(standard_deviation([15, 15, 15, 14, 16]), 0.63)

    def test_2(self):
        self.assertEqual(standard_deviation([1, 2, 3, 4, 5]), 1.41)

    def test_3(self):
        self.assertEqual(
            standard_deviation(
                [-24, 3, -15, 131, 8, 42, 11, -70, 12, 0, 33, 48, 20, 20, 20]
            ),
            41.43,
        )

    def test_4(self):
        self.assertEqual(standard_deviation([-10, -1, -100]), 44.70)

    def test_5(self):
        self.assertEqual(standard_deviation([18, 18, 18]), 0)

    def test_6(self):
        self.assertEqual(standard_deviation([2, 7, 14, 22, 30]), 10.08)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Standard Deviation](https://edabit.com/challenge/frC4AdY2u4tm9aTRz)
