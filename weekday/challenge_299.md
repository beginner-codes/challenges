# Challenge 299 - Operations

Write a function that does the following things: adding, subtracting, dividing, or multiplying values. All you have to do is look at the variable, do some string to integer conversions use some if conditionals, and combine them based on the operation.

The numbers and operation will be given as a string, and you should return the value as a string as well.

## Examples
```python
operation("1", "2", "add" ) ➞ "3"

operation("4", "5", "subtract") ➞ "-1"

operation("6", "3", "divide") ➞ "2"
```
## Notes

- The numbers and operation will be given as a string, and you should also return the value as a string.
- If the answer is undefined, return `"undefined"` (e.g. dividing by zero).
- For divide go ahead and round down to an integer.

## Notes

- Make sure to only capitalize the first letter of each name.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def operation(operand_a: str, operand_b: str, operator: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(operation("1", "2", "add"), "3")

    def test_2(self):
        self.assertEqual(operation("1", "-20", "add"), "-19")

    def test_3(self):
        self.assertEqual(operation("9", "0", "divide"), "undefined")

    def test_4(self):
        self.assertEqual(operation("10", "10", "multiply"), "100")

    def test_5(self):
        self.assertEqual(operation("-10", "-10", "multiply"), "100")

    def test_6(self):
        self.assertEqual(operation("10", "10", "subtract"), "0")

    def test_7(self):
        self.assertEqual(operation("0", "0", "subtract"), "0")

    def test_8(self):
        self.assertEqual(operation("0", "1", "divide"), "0")

    def test_9(self):
        self.assertEqual(operation("0", "25415", "divide"), "0")

    def test_10(self):
        self.assertEqual(
            operation(
                operation("10", "10", "multiply"),
                operation("10", "10", "add"),
                "divide",
            ),
            "5",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Operations](https://edabit.com/challenge/aoN2XoAfQzPQeRNRt)
