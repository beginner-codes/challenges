# Challenge 296 - International Greetings

Suppose you have a guest list of students and the country they are from, stored as key-value pairs in a dictionary.
```
GUEST_LIST = {
    "Randy": "Germany",
    "Karla": "France",
    "Wendy": "Japan",
    "Norman": "England",
    "Sam": "Argentina"
}
```
Write a function that takes in a name and returns a name tag, that should read:
```
"Hi! I'm [name], and I'm from [country]."
```
If the name is not in the dictionary, return:
```
"Hi! I'm a guest."
```
## Examples
```python
greeting("Randy") ➞ "Hi! I'm Randy, and I'm from Germany."

greeting("Sam") ➞ "Hi! I'm Sam, and I'm from Argentina."

greeting("Monti") ➞ "Hi! I'm a guest."
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def greeting(name: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(greeting("Randy"), "Hi! I'm Randy, and I'm from Germany.")

    def test_2(self):
        self.assertEqual(greeting("Sam"), "Hi! I'm Sam, and I'm from Argentina.")

    def test_3(self):
        self.assertEqual(greeting("Monti"), "Hi! I'm a guest.")

    def test_4(self):
        self.assertEqual(greeting("Trudy"), "Hi! I'm a guest.")

    def test_5(self):
        self.assertEqual(greeting("Wendy"), "Hi! I'm Wendy, and I'm from Japan.")


if __name__ == "__main__":
    unittest.main()

```
## Credits

Found on Edabit: [International Greetings](https://edabit.com/challenge/vAS4Hp4wzSEnQs3tZ)
