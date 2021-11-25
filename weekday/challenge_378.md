# Challenge 378 - Let's Talk Like a Monkey 🐵

Create a function that takes a string and returns it translated into monkey language. You have to figure out their language from test cases.

## Examples
```python
monkey_talk("Beginner Codes") ➞ "Ook ook."

monkey_talk("Hello") ➞ "Ook."

monkey_talk("Matt") ➞ "Ook."

monkey_talk("Everyone") ➞ "Eek."

monkey_talk("Programming is Amazing") ➞ "Ook eek eek."
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def monkey_talk(phrase: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(monkey_talk("Beginner Codes"), "Ook ook.")

    def test_2(self):
        self.assertEqual(monkey_talk("Programming is Amazing"), "Ook eek eek.")

    def test_3(self):
        self.assertEqual(monkey_talk("Matt"), "Ook.")

    def test_4(self):
        self.assertEqual(monkey_talk("Hello"), "Ook.")

    def test_5(self):
        self.assertEqual(monkey_talk("you are so beautiful"), "Ook eek ook ook.")

    def test_6(self):
        self.assertEqual(monkey_talk("Everyone"), "Eek.")

    def test_7(self):
        self.assertEqual(monkey_talk("Hello Everyone"), "Ook eek.")

    def test_8(self):
        self.assertEqual(monkey_talk("Everyone Hello"), "Eek ook.")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Let's Talk Like a Monkey 🐵](https://edabit.com/challenge/TAhuay457cw5AekBe)
