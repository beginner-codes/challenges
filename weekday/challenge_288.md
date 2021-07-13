# Challenge 288 - Valid Division

Create a function that takes a division equation d and checks if it will return a whole number without decimals after dividing.

## Examples
```python
valid_division("6/3") ➞ True

valid_division("30/25") ➞ False

valid_division("0/3") ➞ True
```
## Notes

- Return `"invalid"` if division by zero.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Union
import unittest


def valid_division(string: str) -> Union[bool, str]:
    return True  # Put your code here!!!
    

class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(valid_division("6/3"), True)

    def test_2(self):
        self.assertEqual(valid_division("30/25"), False)
        
    def test_3(self):
        self.assertEqual(valid_division("0/3"), True)
        
    def test_4(self):
        self.assertEqual(valid_division("1/3"), False)
        
    def test_5(self):
        self.assertEqual(valid_division("49/7"), True)
    
    def test_6(self):
        self.assertEqual(valid_division("3/0"), "invalid")
       
    def test_7(self):
        self.assertEqual(valid_division("123/0"), "invalid")
        

if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Valid Division](https://edabit.com/challenge/MTGTSJvAi2iwd2Ygs)
