# Challenge 635 - The Out-Shuffle

An out-shuffle, also known as an out faro shuffle or a perfect shuffle, is a controlled method for shuffling playing cards. It is performed by splitting the deck into two equal halves and interleaving them together perfectly, with the condition that the top card of the deck remains in place.

Using an array to represent a deck of cards, an out-shuffle looks like:
```javascript
[1, 2, 3, 4, 5, 6, 7, 8] ➞ [1, 5, 2, 6, 3, 7, 4, 8]
// Card 1 remains in the first position.
```
If we repeat the process, the deck eventually returns to original order.
```
Shuffle 1:
[1, 2, 3, 4, 5, 6, 7, 8] ➞ [1, 5, 2, 6, 3, 7, 4, 8]

Shuffle 2:
[1, 5, 2, 6, 3, 7, 4, 8] ➞ [1, 3, 5, 7, 2, 4, 6, 8]

Shuffle 3:
[1, 3, 5, 7, 2, 4, 6, 8] ➞ [1, 2, 3, 4, 5, 6, 7, 8]
// Back where we started.
```
Write a function that takes a positive even integer representing the number of the cards in a deck, and returns the number of out-shuffles required to return the deck to its original order.

## Examples
```python
shuffle_count(8) ➞ 3

shuffle_count(14) ➞ 12

shuffle_count(52) ➞ 8
```
## Notes

-  The number of cards is always even and greater than one. Thus, the smallest possible deck size is two.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def shuffle_count(num_cards: int) -> int:
    return 0  # Put your code here!!!


test(635, shuffle_count)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            104
        ],
        "return": 51
    },
    {
        "args": [
            52
        ],
        "return": 8
    },
    {
        "args": [
            14
        ],
        "return": 12
    },
    {
        "args": [
            208
        ],
        "return": 66
    },
    {
        "args": [
            8
        ],
        "return": 3
    }
]
```
## Credits

Found on Edabit: [The Out-Shuffle](https://edabit.com/challenge/KLke67efuam6ajLrt)
