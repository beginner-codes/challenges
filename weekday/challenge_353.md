# Challenge 353 - Just Another Sum Problem But...

Ok, the challenge is kind of easy, right?

The problem is not adding, the problem is that the numbers are not in order, create a function that organizes the numbers and adds the numbers in the range between `X` and `Y`.

Here is an example:
```python
X = -10 | Y=1
```
So this will be the range of numbers:
```python
-10, -9, -8, -7, -6, -5, -4, -3, -2, -1, 0, 1
```
This will be your result:
```python
-54
```
You must sum a number range between `X` and `Y` to get the result.

Remember, `X` and `Y` are disorganized, so to get to the result you know what you have to do.

## Examples
```python
just_another_sum_problem(-10, 1) ➞ -54

just_another_sum_problem(-20, 5) ➞ -195

just_another_sum_problem(90, 45) ➞ 3105
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def just_another_sum_problem(a: int, b: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(just_another_sum_problem(1, -10), -54)

    def test_2(self):
        self.assertEqual(just_another_sum_problem(-20, 5), -195)

    def test_3(self):
        self.assertEqual(just_another_sum_problem(-40, 20), -610)

    def test_4(self):
        self.assertEqual(just_another_sum_problem(20, -100), -4840)

    def test_5(self):
        self.assertEqual(just_another_sum_problem(-15, 3), -114)

    def test_6(self):
        self.assertEqual(just_another_sum_problem(-8, 4), -26)

    def test_7(self):
        self.assertEqual(just_another_sum_problem(13, -1000000000), -500000000499999909)

    def test_8(self):
        self.assertEqual(just_another_sum_problem(7, 1000000000), 500000000499999979)

    def test_9(self):
        self.assertEqual(just_another_sum_problem(90, 45), 3105)

    def test_10(self):
        self.assertEqual(just_another_sum_problem(100, 58), 3397)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Just Another Sum Problem But...](https://edabit.com/challenge/XGKSYNExDBRWLzDmm)
