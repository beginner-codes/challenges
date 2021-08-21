# Challenge 317 - Basic Arithmetic Operations on a String Number

Create a function to perform basic arithmetic operations that includes addition, subtraction, multiplication and division on a string number (e.g. `"12 + 24"` or `"23 - 21"` or `"12 / 12"` or `"12 * 21"`).

Here, we have 1 followed by a space, operator followed by another space and 2. For the challenge, we are going to have only two numbers between 1 valid operator. The return value should be a number.

In case of division, whenever the second number equals "0" return -1.

For example:
```python
"15 / 0"  ➞ -1
```
## Examples
```python
arithmetic_operation("12 + 12") ➞ 24 # 12 + 12 = 24

arithmetic_operation("12 - 12") ➞ 24 # 12 - 12 = 0

arithmetic_operation("12 * 12") ➞ 144#/ 12 * 12 = 144

arithmetic_operation("12 / 0") ➞ -1 # 12 / 0 = -1
```
## Notes

- All the inputs are only integers.
- The operators are `*`, `-`, `+`, and `/`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def arithmetic_operation(equation: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(arithmetic_operation("12 + 12"), 24)

    def test_2(self):
        self.assertEqual(arithmetic_operation("22 - 12"), 10)

    def test_3(self):
        self.assertEqual(arithmetic_operation("100 * 12"), 1200)

    def test_4(self):
        self.assertEqual(arithmetic_operation("120 // 10"), 12)

    def test_5(self):
        self.assertEqual(arithmetic_operation("122 // 0"), -1)

    def test_6(self):
        self.assertEqual(arithmetic_operation("10 * 20"), 200)

    def test_7(self):
        self.assertEqual(arithmetic_operation("10 - 10"), 0)

    def test_8(self):
        self.assertEqual(arithmetic_operation("10 - 12"), -2)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Basic Arithmetic Operations on a String Number](https://edabit.com/challenge/peezjw73G8BBGfHdW)
