# Challenge 450 - You Sunk My Battleship!

Remember the game Battleship? Ships are floating in a matrix. You have to fire torpedoes at their suspected coordinates, to try and hit them.

Create a function that takes a list of lists (matrix) and a coordinate as a string. If the coordinate contains only water `"."`, return `"splash"` and if the coordinate contains a ship `"*"`, return `"BOOM"`.

## Examples
```python
[
  [".", ".", ".", "*", "*"],
  [".", "*", ".", ".", "."],
  [".", "*", ".", ".", "."],
  [".", "*", ".", ".", "."],
  [".", ".", "*", "*", "."],
]

fire(matrix, "A1") ➞ "splash"

fire(matrix, "A4") ➞ "BOOM"

fire(matrix, "D2") ➞ "BOOM"
```
## Notes

- The provided matrix is always a square.
- The provided matrix will not be larger than `5 * 5` (`A1 * E5`).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
    {
        "args": [
            [
                [".", ".", ".", "*", "*"],
                [".", "*", ".", ".", "."],
                [".", "*", ".", ".", "."],
                [".", "*", ".", ".", "."],
                [".", ".", "*", "*", "."],
            ],
            "A1"
        ],
        "return": "splash"
    },
    {
        "args": [
            [
                [".", ".", ".", "*", "*"],
                [".", "*", ".", ".", "."],
                [".", "*", ".", ".", "."],
                [".", "*", ".", ".", "."],
                [".", ".", "*", "*", "."],
            ],
            "C2"
        ],
        "return": "BOOM"
    },
    {
        "args": [
            [
                [".", "."],
                ["*", "*"]
            ],
            "B1"
        ],
        "return": "BOOM"
    },
    {
        "args": [
            [
                [".", "."],
                ["*", "*"]
            ],
            "A2"
        ],
        "return": "splash"
    },
    {
        "args": [
            [
                ["*", ".", "."],
                [".", ".", "."],
                [".", "*", "*"],
            ],
            "C3"
        ],
        "return": "BOOM"
    }
]
```
## Credits

Found on Edabit: [You Sunk My Battleship!](https://edabit.com/challenge/cGqjxKhNqZPZ76zac)
