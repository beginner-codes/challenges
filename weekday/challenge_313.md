# Challenge 313 - Which Function Returns the Larger Number?

Your function will be passed two functions, `f` and `g`, that don't take any parameters. Your function has to call them, and return a string which indicates which function returned the larger number.

- If `f` returns the larger number, return the string `"f"`.
- If `g` returns the larger number, return the string `"g"`.
- If the functions return the same number, return the string `"neither"`.

## Examples
```python
which_is_larger(lambda: 5, lambda: 10) ➞ "g"

which_is_larger(lambda: 25,  lambda: 25) ➞ "neither"

which_is_larger(lambda: 505050, lambda: 5050) ➞ "f"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from typing import Callable
import unittest


def which_is_larger(f: Callable[[], int], g: Callable[[], int]) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(which_is_larger(lambda: 5, lambda: 10), "g")

    def test_2(self):
        self.assertEqual(which_is_larger(lambda: 10, lambda: 5), "f")

    def test_3(self):
        self.assertEqual(which_is_larger(lambda: 25, lambda: 25), "neither")

    def test_4(self):
        self.assertEqual(which_is_larger(lambda: -100, lambda: -100), "neither")

    def test_5(self):
        self.assertEqual(which_is_larger(lambda: -100, lambda: 0), "g")

    def test_6(self):
        self.assertEqual(which_is_larger(lambda: 505050, lambda: 5050), "f")

    def test_7(self):
        self.assertEqual(which_is_larger(lambda: 100, lambda: 1000), "g")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Which Function Returns the Larger Number?](https://edabit.com/challenge/Rg26hsPPXXqpho3g2)
