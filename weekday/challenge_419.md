# Challenge 419 - Sums of Parts

Let us consider this example:
```python
ls = [0, 1, 3, 6, 10]
```
Its following parts:
```python
[0, 1, 3, 6, 10]
[1, 3, 6, 10]
[3, 6, 10]
[6, 10]
[10]
[]
```
The corresponding sums of each part in a list are: `[20, 20, 19, 16, 10, 0]`

The function `parts_sums` will take as parameters a list of numbers and return a list of the sums of its parts as defined above.

Other Examples:
```python
parts_sums([1, 2, 3, 4, 5, 6])
-> [21, 20, 18, 15, 11, 6, 0]

parts_sums([744125, 935, 407, 454, 430, 90, 144, 6710213, 889, 810, 2579358])
-> [10037855, 9293730, 9292795, 9292388, 9291934, 9291504, 9291414, 9291270, 2581057, 2580168, 2579358, 0]
```
## Notes

- Take a look at performance: some lists have thousands of elements.
- Please ask before translating.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def parts_sum(numbers: list[int]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(parts_sum([]), [0])

    def test_2(self):
        self.assertListEqual(parts_sum([0, 1, 3, 6, 10]), [20, 20, 19, 16, 10, 0])

    def test_3(self):
        self.assertListEqual(parts_sum([1, 2, 3, 4, 5, 6]), [21, 20, 18, 15, 11, 6, 0])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Codewars: [Sums of Parts](https://www.codewars.com/kata/5ce399e0047a45001c853c2b)
