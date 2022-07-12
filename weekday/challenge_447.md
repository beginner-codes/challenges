# Challenge 447 - Is It the Same Upside Down?

The number `6090609` has a special property: if you turn the number upside down (imagine rotating your screen 180 degrees), you get `6090609` again.

Write a function that takes a string on the digits `0`, `6`, `9` and decides if the number is the same upside down.

## Examples
```python
same_upsidedown("6090609") ➞ True

same_upsidedown("9669") ➞ False
# Becomes 6996 when upside down.

same_upsidedown("69069069") ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
  {"args": ["9"], "return": false},
  {"args": ["0"], "return": true},
  {"args": ["6090609"], "return": true},
  {"args": ["9669"], "return": false},
  {"args": ["69069069"], "return": true},
  {"args": ["60906096090609"], "return": true},
  {"args": ["966909669"], "return": false},
  {"args": ["6000000009"], "return": true},
  {"args": ["6666660999999"], "return": true},
  {"args": ["96666660999999"], "return": false}
]
```
## Credits

Found on Edabit: [Is It the Same Upside Down?](https://edabit.com/challenge/LDQvCxTPv4iiY8B2A)
