# Challenge 252 - The Out-Shuffle

An out-shuffle, also known as an out faro shuffle or a perfect shuffle, is a controlled method for shuffling playing cards. It is performed by splitting the deck into two equal halves and interleaving them together perfectly, with the condition that the top card of the deck remains in place.

Using a list to represent a deck of cards, an out-shuffle looks like:
```python
[1, 2, 3, 4, 5, 6, 7, 8] ➞ [1, 5, 2, 6, 3, 7, 4, 8]
# Card 1 remains in the first position.
```
If we repeat the process, the deck eventually returns to original order.

Shuffle 1:
```python
[1, 2, 3, 4, 5, 6, 7, 8] ➞ [1, 5, 2, 6, 3, 7, 4, 8]
```
Shuffle 2:
```python
[1, 5, 2, 6, 3, 7, 4, 8] ➞ [1, 3, 5, 7, 2, 4, 6, 8]
```
Shuffle 3:
```python
[1, 3, 5, 7, 2, 4, 6, 8] ➞ [1, 2, 3, 4, 5, 6, 7, 8]
# Back where we started.
```
Write a function that takes a positive even integer representing the number of the cards in a deck and returns the number of out-shuffles required to return the deck to its original order.

## Examples
```python
shuffle_count(8) ➞ 3

shuffle_count(14) ➞ 12

shuffle_count(52) ➞ 8
```
## Notes

- The number of cards is always even and greater than one. Thus, the smallest possible deck size is two.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def shuffle_count(num_cards: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(shuffle_count(2), 1)

    def test_2(self):
        self.assertEqual(shuffle_count(8), 3)

    def test_3(self):
        self.assertEqual(shuffle_count(14), 12)

    def test_4(self):
        self.assertEqual(shuffle_count(26), 20)

    def test_5(self):
        self.assertEqual(shuffle_count(52), 8)

    def test_6(self):
        self.assertEqual(shuffle_count(70), 22)

    def test_7(self):
        self.assertEqual(shuffle_count(104), 51)

    def test_8(self):
        self.assertEqual(shuffle_count(208), 66)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [The Out-Shuffle](https://edabit.com/challenge/oJs9RW9rjQosxT8Xu)
