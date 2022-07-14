# Challenge 431 - Food for Everyone!

Create a Person class which will have three properties:

- Name
- List of foods they like
- List of foods they hate

In this class, create the method `taste`:

- It will take in a food name as a string.
- Return `"{person_name} eats the {food_name}"`.
- If the food is in the person's like list, add `"and loves it!"` to the end.
- If it is in the person's hate list, add `"and hates it!"` to the end.
- If it is in neither list, simply add an exclamation mark to the end.

## Examples
```python
p1 = Person("Sam", ["ice cream"], ["carrots"])
p1.taste("ice cream") ➞ "Sam eats the ice cream and loves it!"

p1.taste("cheese") ➞ "Sam eats the cheese!"

p1.taste("carrots") ➞ "Sam eats the carrots and hates it!"
```
## Notes

- A person can have an empty list for foods they hate and/or love.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from abc import ABC, abstractmethod
import unittest


class AbstractPerson(ABC):
    @abstractmethod
    def __init__(self, name: str, likes: list[str], dislikes: list[str]):
        ...

    @abstractmethod
    def taste(self, food: str) -> str:
        ...


class Person(AbstractPerson):
    """Put your code here!!!"""


class Tests(unittest.TestCase):
    def setUp(self):
        self.p1 = Person(
            "Sam",
            ["ice cream", "pie", "apples"],
            ["carrots", "bananas", "cheese", "lettuce"],
        )
        self.p2 = Person(
            "Mitchell",
            [],
            [
                "brocolli",
                "lettuce",
                "cheese",
                "pie",
                "apples",
                "bananas",
                "ice cream",
                "carrots",
            ],
        )

    def test_1(self):
        self.assertEqual(
            self.p1.taste("ice cream"), "Sam eats the ice cream and loves it!"
        )

    def test_2(self):
        self.assertEqual(self.p1.taste("carrots"), "Sam eats the carrots and hates it!")

    def test_3(self):
        self.assertEqual(self.p1.taste("brocolli"), "Sam eats the brocolli!")

    def test_4(self):
        self.assertEqual(self.p1.taste("lettuce"), "Sam eats the lettuce and hates it!")

    def test_5(self):
        self.assertEqual(self.p1.taste("cheese"), "Sam eats the cheese and hates it!")

    def test_6(self):
        self.assertEqual(self.p1.taste("pie"), "Sam eats the pie and loves it!")

    def test_7(self):
        self.assertEqual(self.p1.taste("apples"), "Sam eats the apples and loves it!")

    def test_8(self):
        self.assertEqual(self.p1.taste("bananas"), "Sam eats the bananas and hates it!")

    def test_9(self):
        self.assertEqual(
            self.p2.taste("ice cream"), "Mitchell eats the ice cream and hates it!"
        )

    def test_10(self):
        self.assertEqual(
            self.p2.taste("carrots"), "Mitchell eats the carrots and hates it!"
        )

if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Food for Everyone!](https://edabit.com/challenge/iRvRtg2xxL9BnSEvf)
