# Challenge 298 - Name Classes

Write a class called `Name` and create the following attributes:

- An attribute called `fname`
- An attribute called `lname`
- An attribute called `fullname` which returns the first and last names.
- An attribute called `initials` which returns the first letters of the first and last name. Put a `.` between the two letters.

*Remember to allow the attributes fname and lname to be accessed individually as well.*

## Examples
```python
a1 = Name("john", "SMITH")
a1.fname ➞ "John"

a1.lname ➞ "Smith"

a1.fullname ➞ "John Smith"

a1.initials ➞ "J.S"
```
## Notes

- Make sure to only capitalize the first letter of each name.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


class Name:
    def __init__(self, first: str, last: str):
        """Put your code here!!!"""


class Tests(unittest.TestCase):
    def __init__(self):
        self.a1 = Name("john", "SMITH")
        self.a2 = Name("sARah", "fRolliE")

    def test_1(self):
        self.assertEqual(self.a1.fname, "John")

    def test_2(self):
        self.assertEqual(self.a1.lname, "Smith")

    def test_3(self):
        self.assertEqual(self.a1.fullname, "John Smith")

    def test_4(self):
        self.assertEqual(self.a1.initials, "J.S")

    def test_5(self):
        self.assertEqual(self.a2.fname, "Sarah")

    def test_6(self):
        self.assertEqual(self.a2.lname, "Frollie")

    def test_7(self):
        self.assertEqual(self.a2.fullname, "Sarah Frollie")

    def test_8(self):
        self.assertEqual(self.a2.initials, "S.F")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Name Classes](https://edabit.com/challenge/kbtju9wk5pjGYMmHF)
