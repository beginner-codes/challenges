# Challenge 289 - Emphasize the Words

The challenge is to recreate the functionality of the `title()` method into a function called `emphasize()`. The `title()` method capitalises the first letter of every word and lowercases all of the other letters in the word.

## Examples
```python
emphasize("hello world") ➞ "Hello World"

emphasize("GOOD MORNING") ➞ "Good Morning"

emphasize("99 red balloons!") ➞ "99 Red Balloons!"
```
## Notes

- You won't run into any issues when dealing with numbers in strings.
- Please don't use the `title()` method directly

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import inspect
import unittest


def emphasize(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(emphasize("hello world"), "Hello World")

    def test_2(self):
        self.assertEqual(emphasize("GOOD MORNING"), "Good Morning")

    def test_3(self):
        self.assertEqual(emphasize("99 red balloons!"), "99 Red Balloons!")

    def test_4(self):
        self.assertEqual(emphasize("1 2 3 4 5 6 7 8 9"), "1 2 3 4 5 6 7 8 9")

    def test_5(self):
        self.assertEqual(emphasize(""), "")

    def test_6(self):
        self.assertEqual(emphasize("joshua senoron"), "Joshua Senoron")

    def test_7(self):
        self.assertNotEqual(str.title, emphasize)
        self.assertNotIn(".title", inspect.getsource(emphasize))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Emphasize the Words](https://edabit.com/challenge/K5277r6RmsJRSz27t)
