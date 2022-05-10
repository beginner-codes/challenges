# Challenge 454 - Unfair Hurdles

Unfair hurdles are hurdles which are either too high, or way too close together.

Create a function which takes in a list of strings representing hurdles, and return whether they are unfair. For the purposes of this challenge, unfair hurdles are:

- At least 4 characters tall.
- Strictly less than 4 spaces apart.

## Examples
```python
# Hurdle are good distance apart but are way too tall.

is_unfair_hurdle([
  "#    #    #    #",
  "#    #    #    #",
  "#    #    #    #",
  "#    #    #    #"
]) ➞ True


# Hurdles are a fine height but are way too close together.

is_unfair_hurdle([
  "#  #  #  #",
  "#  #  #  #",
  "#  #  #  #"
]) ➞ True


# These hurdles are mighty splendid.

is_unfair_hurdle([
  "#      #      #      #",
  "#      #      #      #"
]) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
    {
        "args": [
            5,
            [
                5,
                4.2,
                3,
                3.5,
                6,
                4,
                6,
                8,
                1
            ]
        ],
        "return": 3
    },
    {
        "args": [
            10,
            [
                5,
                4.2,
                3,
                3.5,
                6,
                4,
                6,
                8,
                1
            ]
        ],
        "return": 3
    },
    {
        "args": [
            20,
            [
                5,
                4.2,
                3,
                3.5,
                6,
                4,
                6,
                8,
                1
            ]
        ],
        "return": 6
    },
    {
        "args": [
            100,
            [
                5,
                4.2,
                3,
                3.5,
                6,
                4,
                6,
                8,
                1
            ]
        ],
        "return": 8
    },
    {
        "args": [
            5,
            [
                0,
                1,
                2.5,
                0.8
            ]
        ],
        "return": 1
    }
]
```
## Credits

Found on Edabit: [Climbing Competition](https://edabit.com/challenge/Q7oecYfjkq7tHwPoA)
