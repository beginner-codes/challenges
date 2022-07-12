# Challenge 367 - The Fibonacci Number

Create a function that, given a number, returns the corresponding value of that index in the Fibonacci series.

The Fibonacci Sequence is the series of numbers:
```python
1, 1, 2, 3, 5, 8, 13, 21, 34, ...
```
The next number is found by adding the two numbers before it:

- The 2 is found by adding the two numbers before it (`1+1`).
- The 3 is found by adding the two numbers before it (`1+2`).
- The 5 is (`2+3`), and so on!

## Examples
```python
fibonacci(3) ➞ 3

fibonacci(7) ➞ 21

fibonacci(12) ➞ 233
```
## Notes

- The first number in the sequence starts at 1 (not 0).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def fibonacci(index: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(fibonacci(3), 3)

    def test_2(self):
        self.assertEqual(fibonacci(7), 21)

    def test_3(self):
        self.assertEqual(fibonacci(12), 233)

    def test_4(self):
        self.assertEqual(fibonacci(0), 1)

    def test_5(self):
        self.assertEqual(fibonacci(1), 1)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [The Fibonacci Number](https://edabit.com/challenge/8Ko5tPg8Ch5SRCAhA)
