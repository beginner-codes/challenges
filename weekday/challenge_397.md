# Challenge 397 - Turn That Frown Upside Down

It is important to be happy! Therefore, you must create a function that takes a sentence containing sad faces and turn them into happy ones! This involves changing only the mouths.

- Sad face examples: `:(` `8(` `x(` `;(`
- Happy face examples: `:)` `8)` `x)` `;)`
- Make sure to only change the face if there are eyes before them, `round(3.4)` wouldn't become `round)3.4)` (for example).

## Examples
```python
make_happy("My current mood: :(") ➞ "My current mood: :)"

make_happy("I was hungry 8(") ➞ "I was hungry 8)"

make_happy("print('x(')") ➞ "print('x)')"
```
## Notes

- Faces such as `:(((((((` are not included.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def make_happy(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(make_happy("My current mood: :("), "My current mood: :)")

    def test_2(self):
        self.assertEqual(make_happy("I was hungry 8("), "I was hungry 8)")

    def test_3(self):
        self.assertEqual(make_happy('print("x(")'), 'print("x)")')

    def test_4(self):
        self.assertEqual(make_happy("I'm thirsty ;("), "I'm thirsty ;)")

    def test_5(self):
        self.assertEqual(make_happy("(((:())))"), "(((:)))))")

    def test_6(self):
        self.assertEqual(make_happy("I am :( :( 8( :)"), "I am :) :) 8) :)")

    def test_7(self):
        self.assertEqual(make_happy("l"), "l")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Turn That Frown Upside Down](https://edabit.com/challenge/mCNwMqca9R3hBY6fY)
