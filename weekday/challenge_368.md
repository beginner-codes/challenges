# Challenge 368 - Encoded String Parse

Create a function which takes in an encoded string and returns a dictionary according to the following example:

## Examples
```python
parse_code("John000Doe000123") ➞ {
  "first_name": "John",
  "last_name": "Doe",
  "id": "123"
}

parse_code("michael0smith004331") ➞ {
  "first_name": "michael",
  "last_name": "smith",
  "id": "4331"
}

parse_code("Thomas00LEE0000043") ➞ {
  "first_name": "Thomas",
  "last_name": "LEE",
  "id": "43"
}
```
## Notes

- The string will always be in the same format: `first name`, `last name`, and `id` with zeros between them.
- `id` numbers will not contain any zeros.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def parse_code(encoded_string: str) -> dict[str, str]:
    return {}  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            parse_code("John000Doe000123"),
            {"first_name": "John", "last_name": "Doe", "id": "123"},
        )

    def test_2(self):
        self.assertEqual(
            parse_code("Michael0Smith004331"),
            {"first_name": "Michael", "last_name": "Smith", "id": "4331"},
        )

    def test_3(self):
        self.assertEqual(
            parse_code("Thomas0000Lee0000045553"),
            {"first_name": "Thomas", "last_name": "Lee", "id": "45553"},
        )

    def test_4(self):
        self.assertEqual(
            parse_code("a0b01"), {"first_name": "a", "last_name": "b", "id": "1"}
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Encoded String Parse](https://edabit.com/challenge/7vN8ZRw43yuWNoy3Y)
