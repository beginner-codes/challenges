# Challenge 359 - Book Shelf

Create a `Book` class that has two attributes:

- `.title`
- `.author`

and two methods:

- A method named `.get_title()` that returns: `"Title: "` + the instance title.
- A method named `.get_author()` that returns: `"Author: "` + the instance author.

For instance, if I instantiated the following book using this Book class:
```
Harry Potter - J.K. Rowling (HP)
```
I would get the following attributes and methods:

## Examples
```python
HP.title ➞ "Harry Potter"
HP.author ➞ "J.K. Rowling"
HP.get_title() ➞ "Title: Harry Potter"
HP.get_author() ➞ "Author: J.K. Rowling"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


class Book:
    def __init__(self, title: str, author: str):
        """Put your code here!!!"""


class Tests(unittest.TestCase):
    def setUp(self) -> None:
        self.PP = Book("Pride and Prejudice", "Jane Austen")

    def test_1(self):
        self.assertEqual(self.PP.title, "Pride and Prejudice")

    def test_2(self):
        self.assertEqual(self.PP.author, "Jane Austen")

    def test_3(self):
        self.assertEqual(self.PP.get_title(), "Title: Pride and Prejudice")

    def test_4(self):
        self.assertEqual(self.PP.get_author(), "Author: Jane Austen")
        

if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Book Shelf](https://edabit.com/challenge/uK4Dw7Pise5uCfKqo)
