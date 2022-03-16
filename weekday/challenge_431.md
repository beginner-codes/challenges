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

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def pirates_killed(gold: list[int], thresholds: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(pirates_killed([3, 5, 8, 3, 4], [10, 4, 2, 5, 5]))

    def test_2(self):
        self.assertTrue(pirates_killed([3, 5, 8, 3, 4], [10, 4, 2, 5, 1]))

    def test_3(self):
        self.assertFalse(pirates_killed([3, 3, 10], [7, 7, 0]))

    def test_4(self):
        self.assertTrue(pirates_killed([3, 3, 10], [6, 6, 0]))

    def test_5(self):
        self.assertFalse(pirates_killed([3, 3, 3], [0, 0, 0]))

    def test_6(self):
        self.assertTrue(pirates_killed([3, 3, 4, 4], [0, 0, 1, 1]))

    def test_7(self):
        self.assertFalse(pirates_killed([3, 3, 4, 4], [1, 1, 0, 0]))

    def test_8(self):
        self.assertTrue(pirates_killed([3, 3, 4, 4], [0, 0, 0, 1]))

    def test_9(self):
        self.assertTrue(pirates_killed([3, 3, 4, 4, 5], [0, 0, 0, 1, 1]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Food for Everyone!](https://edabit.com/challenge/iRvRtg2xxL9BnSEvf)
