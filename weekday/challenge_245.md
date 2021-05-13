# Challenge 245 - Cricket Balls to Overs!

In cricket, an over consists of six deliveries a bowler bowls from one end. Create a function that takes the number of balls bowled by a bowler and calculates the number of overs and balls bowled by him/her. Return the value as a float, in the format overs.balls.

## Examples
```python
total_overs(2400) ➞ 400

total_overs(164) ➞ 27.2
# 27 overs and 2 balls were bowled by the bowler.

total_overs(945) ➞ 157.3
# 157 overs and 3 balls were bowled by the bowler.

total_overs(5) ➞ 0.5
```
## Notes

- The number following the decimal point represents the balls remaining after the last over. Therefore, it will only ever have a value of 1-5.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def total_overs(balls: int) -> float:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(total_overs(2400), 400)

    def test_2(self):
        self.assertEqual(total_overs(164), 27.2)

    def test_3(self):
        self.assertEqual(total_overs(945), 157.3)

    def test_4(self):
        self.assertEqual(total_overs(5), 0.5)

    def test_5(self):
        self.assertEqual(total_overs(7), 1.1)

    def test_6(self):
        self.assertEqual(total_overs(15), 2.3)

    def test_7(self):
        self.assertEqual(total_overs(0), 0)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Cricket Balls to Overs!](https://edabit.com/challenge/guR6aa2zytfZvywMS)
