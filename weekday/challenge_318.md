# Challenge 318 - Sum of v0w3ls

Create a function that takes a string and returns the sum of vowels, where some vowels are considered numbers.
```
Vowel	Number
A	    4
E	    3
I	    1
O	    0
U	    0
```
## Examples
```python
sum_of_vowels("Let\'s test this function.") ➞ 8

sum_of_vowels("Do I get the correct output?") ➞ 10
```
## Notes

- Vowels are case-insensitive (e.g. `A = 4` and `a = 4`).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def sum_of_vowels(string: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sum_of_vowels("Let's test this function."), 8)

    def test_2(self):
        self.assertEqual(sum_of_vowels("Do I get the correct output?"), 10)

    def test_3(self):
        self.assertEqual(sum_of_vowels("Will you still need me, will you still feed me when I'm 64?"), 26)

    def test_4(self):
        self.assertEqual(
            sum_of_vowels("The greatest glory in living lies not in never falling, but in rising every time we fall."),
            52
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum of v0w3ls](https://edabit.com/challenge/6NoaFGKJgRW6oXhLC)
