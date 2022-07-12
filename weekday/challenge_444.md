# Challenge 444 - Drink Sorting

You will be given a list of drinks, with each drink being a dictionary with two properties: `name` and `price`. Create a function that has the drinks list as an argument and returns the drinks dictionaries sorted by price in ascending order.

Assume that the following array of drink objects needs to be sorted:
```python
drinks = [
  {"name": "lemonade", "price": 50},
  {"name": "lime", "price": 10}
]
```
The output of the sorted drinks object will be:

## Examples
```python
sort_drinks_by_price(drinks) ➞ [{"name": "lime", "price": 10}, {"name": "lemonade", "price": 50}]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
  {
    "args": [[{"name": "lemonade", "price": 90}, {"name": "lime", "price": 432}, {"name": "peach", "price": 23}]],
    "return": [{"name": "peach", "price": 23}, {"name": "lemonade", "price": 90}, {"name": "lime", "price": 432}]
  },
  {
    "args": [[{"name": "lemonade", "price": 266}, {"name": "cola", "price": 71}, {"name": "lime", "price": 467}, {"name": "peach", "price": 203}, {"name": "water", "price": 216}]],
    "return": [{"name": "cola", "price": 71}, {"name": "peach", "price": 203}, {"name": "water", "price": 216}, {"name": "lemonade", "price": 266}, {"name": "lime", "price": 467}]
  },
  {
    "args": [[{"name": "lemonade", "price": 467}, {"name": "cola", "price": 486}, {"name": "lime", "price": 469}]],
    "return": [{"name": "lemonade", "price": 467}, {"name": "lime", "price": 469}, {"name": "cola", "price": 486}]
  },
  {
    "args": [[{"name": "lemonade", "price": 373}, {"name": "cola", "price": 459}, {"name": "lime", "price": 461}]],
    "return": [{"name": "lemonade", "price": 373}, {"name": "cola", "price": 459}, {"name": "lime", "price": 461}]
  }
]
```
## Credits

Found on Edabit: [Drink Sorting](https://edabit.com/challenge/yGBevdRmXvSyTaBSA)
