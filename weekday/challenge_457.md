# Challenge 457 - How Many Shuffles?

An out-shuffle, also known as an out Faro shuffle or a perfect shuffle, is a controlled method for shuffling playing cards. It is performed by splitting the deck into two equal halves and interleaving them together perfectly, with the condition that the top card of the deck remains in place.

Using a list to represent a deck of cards, an out-shuffle looks like:
```python
[1, 2, 3, 4, 5, 6, 7, 8] ➞ [1, 5, 2, 6, 3, 7, 4, 8]
# Card 1 remains in the first position.
```
If we repeat the process, the deck eventually returns to original order:

_Shuffle 1:_
```python
[1, 2, 3, 4, 5, 6, 7, 8] ➞ [1, 5, 2, 6, 3, 7, 4, 8]
```
_Shuffle 2:_
```python
[1, 5, 2, 6, 3, 7, 4, 8] ➞ [1, 3, 5, 7, 2, 4, 6, 8]
```
_Shuffle 3:_
```python
[1, 3, 5, 7, 2, 4, 6, 8] ➞ [1, 2, 3, 4, 5, 6, 7, 8]
# Back where we started.
```
Write a function that takes a positive even integer num representing the number of the cards in a deck, and returns the number of out-shuffles required to return the deck to its original order.

## Examples
```python
shuffle_count(8) ➞ 3

shuffle_count(14) ➞ 12

shuffle_count(52) ➞ 8
```
## Notes

- The number of cards is always greater than zero. Thus, the smallest possible deck size is `2`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
    {
        "args": [
            2
        ],
        "return": 1
    },
    {
        "args": [
            8
        ],
        "return": 3
    },
    {
        "args": [
            14
        ],
        "return": 12
    },
    {
        "args": [
            38
        ],
        "return": 36
    },
    {
        "args": [
            52
        ],
        "return": 8
    },
    {
        "args": [
            70
        ],
        "return": 22
    }
]
```
## Credits

Found on Edabit: [How Many Shuffles?](https://edabit.com/challenge/quMt6typruySiNSAJ)
