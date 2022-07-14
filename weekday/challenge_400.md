# Challenge 400 - Prison Break

A prison can be represented as a list of cells. Each cell contains exactly one prisoner. A `1` represents an unlocked cell and a `0` represents a locked cell.
```python
[1, 1, 0, 0, 0, 1, 0]
```
Starting inside the leftmost cell, you are tasked with seeing how many prisoners you can set free, with a catch. You are the prisoner in the first cell. If the first cell is locked, you cannot free anyone. Each time you free a prisoner, the locked cells become unlocked, and the unlocked cells become locked again.

So, if we use the example above:
```python
[1, 1, 0, 0, 0, 1, 0]
# You free the prisoner in the 1st cell.

[0, 0, 1, 1, 1, 0, 1] 
# You free the prisoner in the 3rd cell (2nd one locked).

[1, 1, 0, 0, 0, 1, 0]
# You free the prisoner in the 6th cell (3rd, 4th and 5th locked).

[0, 0, 1, 1, 1, 0, 1]
# You free the prisoner in the 7th cell - and you are done!
```
Here, we have set free 4 prisoners in total.

Create a function that, given this unique prison arrangement, returns the number of freed prisoners.

## Examples
```python
freed_prisoners([1, 1, 0, 0, 0, 1, 0]) ➞ 4

freed_prisoners([1, 1, 1]) ➞ 1

freed_prisoners([0, 0, 0]) ➞ 0

freed_prisoners([0, 1, 1, 1]) ➞ 0
```
## Notes

- You are the prisoner in the first cell. You must be freed to free anyone else.
- You must free a prisoner in order for the locks to switch. So in the second example where the input is `[1, 1, 1]` after you release the first prisoner, the locks change to `[0, 0, 0]`. Since all cells are locked, you can release no more prisoners.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def freed_prisoners(prisoners: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(freed_prisoners([1, 1, 0, 0, 0, 1, 0]), 4)

    def test_2(self):
        self.assertEqual(freed_prisoners([1, 0, 0, 0, 0, 0, 0]), 2)

    def test_3(self):
        self.assertEqual(freed_prisoners([1, 1, 1, 0, 0, 0]), 2)

    def test_4(self):
        self.assertEqual(freed_prisoners([1, 0, 1, 0, 1, 0]), 6)

    def test_5(self):
        self.assertEqual(freed_prisoners([1, 1, 1]), 1)

    def test_6(self):
        self.assertEqual(freed_prisoners([0, 0, 0]), 0)

    def test_7(self):
        self.assertEqual(freed_prisoners([0, 1, 1, 1]), 0)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Prison Break](https://edabit.com/challenge/SHdu4GwBQehhDm4xT)
