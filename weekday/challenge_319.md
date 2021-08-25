# Challenge 319 - Get Student Most Notes

Create a function that takes a list of student dictionaries and returns a list of most notes they each have for a class.

## Examples
```python
get_student_most_notes([
  {
    "id": 1,
    "name": "Jacek",
    "notes": [5, 3, 4, 2, 5, 5]
  },
  {
    "id": 2,
    "name": "Ewa",
    "notes": [2, 3, 3, 3, 2, 5]
  },
  {
    "id": 3,
    "name": "Zygmunt",
    "notes": [2, 2, 4, 4, 3, 3]
  }
]) ➞ [5, 5, 4]
```

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Union
import unittest


def get_student_most_notes(students: list[dict[str, Union[int, str, list[int]]]]) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            get_student_most_notes(
                [
                    {"id": 1, "name": "Jacek", "notes": [5, 3, 4, 2, 5, 5]},
                    {"id": 2, "name": "Ewa", "notes": [2, 3, 3, 3, 2, 5]},
                    {"id": 3, "name": "Zygmunt", "notes": [2, 2, 4, 4, 3, 3]},
                ]
            ),
            [5, 5, 4],
        )

    def test_2(self):
        self.assertListEqual(
            get_student_most_notes(
                [
                    {"id": 1, "name": "Rochelle", "notes": [0, 0, 3, 3, 5]},
                    {"id": 2, "name": "Robert", "notes": []},
                    {"id": 3, "name": "Hans", "notes": [2, 4, 5]},
                    {"id": 4, "name": "Joel", "notes": [2, 5]},
                    {"id": 5, "name": "Eric", "notes": [3, 5]},
                    {"id": 6, "name": "Cary", "notes": [1, 2, 0, 0]},
                    {"id": 7, "name": "Cary", "notes": [3, 2, 1]},
                    {"id": 8, "name": "Dennis", "notes": [0, 0, 4]},
                    {"id": 9, "name": "Lexi", "notes": [0, 1, 2, 1, 5]},
                    {"id": 10, "name": "Alfie", "notes": [0, 1, 3, 4, 3]},
                ]
            ),
            [5, 0, 5, 5, 5, 2, 3, 4, 5, 4],
        )

    def test_3(self):
        self.assertListEqual(
            get_student_most_notes(
                [
                    {"id": 1, "name": "Max", "notes": [1, 5]},
                    {"id": 2, "name": "Cary", "notes": [0, 5]},
                    {"id": 3, "name": "Lexi", "notes": [2, 0]},
                    {"id": 4, "name": "Joshua", "notes": [1, 2, 2]},
                    {"id": 5, "name": "Hans", "notes": [3, 4, 0, 5, 1]},
                    {"id": 6, "name": "Alfie", "notes": [0, 0, 2, 1, 5]},
                    {"id": 7, "name": "Ralph", "notes": [4, 3, 1, 1, 1]},
                ]
            ),
            [5, 5, 2, 2, 5, 5, 4],
        )

    def test_4(self):
        self.assertListEqual(
            get_student_most_notes(
                [
                    {"id": 1, "name": "Dennis", "notes": [0, 4, 3, 4, 5]},
                    {"id": 2, "name": "Rudolf", "notes": [3, 1]},
                    {"id": 3, "name": "Rudolf", "notes": [2, 4, 4, 5]},
                    {"id": 4, "name": "Dennis", "notes": [2, 5]},
                    {"id": 5, "name": "Rochelle", "notes": [5, 5, 4]},
                    {"id": 6, "name": "John", "notes": [4]},
                    {"id": 7, "name": "Julius", "notes": [2, 1, 4, 4]},
                    {"id": 8, "name": "Cary", "notes": [0, 2, 4, 1, 1]},
                ]
            ),
            [5, 3, 5, 5, 5, 4, 4, 4],
        )

    def test_5(self):
        self.assertListEqual(
            get_student_most_notes(
                [
                    {"id": 1, "name": "Ralph", "notes": [3, 5, 5, 4, 2]},
                    {"id": 2, "name": "Joel", "notes": []},
                    {"id": 3, "name": "Cary", "notes": [0, 5, 0, 4]},
                    {"id": 4, "name": "Noel", "notes": [0, 1, 0, 0]},
                    {"id": 5, "name": "Eric", "notes": [4, 0]},
                    {"id": 6, "name": "Joe", "notes": [4, 3]},
                    {"id": 7, "name": "Lexi", "notes": [1, 3, 0, 5]},
                    {"id": 8, "name": "Max", "notes": []},
                ]
            ),
            [5, 0, 5, 1, 4, 4, 5, 0],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Get Student Top Notes](https://edabit.com/challenge/jt8XTr75xxowgi6KM)
