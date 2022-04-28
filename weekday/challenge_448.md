# Challenge 448 - Wurst Is Better

Wurst is the best. Create a function that takes a string and replaces every mention of any type of sausage with the German word `"Wurst"`, unless—of course—the sausage is already a type of German `"Wurst"` (i.e. `"Bratwurst"`, see below), then leave the sausage name unchanged.

*Types Of Sausages*

- Kielbasa
- Chorizo
- Moronga
- Salami
- Sausage
- Andouille
- Naem
- Merguez
- Gurka
- Snorkers
- Pepperoni

## Rules

- Replace sausages from the list with `"Wurst"`.
- The word `"Wurst"` must be capitalized.

## Examples
```python
wurst_is_better("I like chorizos, but not sausages") ➞ "I like Wursts, but not Wursts"

wurst_is_better("sich die Wurst vom Brot nehmen lassen") ➞ "sich die Wurst vom Brot nehmen lassen"

wurst_is_better("Bratwurst and Rostbratwurst are sausages") ➞ "Bratwurst and Rostbratwurst are Wursts"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
  {
    "args": ["Sausage fests are like salami fests"],
    "return": "Wurst fests are like Wurst fests"
  },
  {
    "args": ["Add the kielbasa and the reserved potatoes and stir through"],
    "return": "Add the Wurst and the reserved potatoes and stir through"
  },
  {
    "args": ["Salami sandwiches, salami and cheese, salami on crackers - I couldn't get enough of the salty, spicy sausage"],
    "return": "Wurst sandwiches, Wurst and cheese, Wurst on crackers - I couldn't get enough of the salty, spicy Wurst"
  },
  {
    "args": ["sich die Wurst vom Brot nehmen lassen"],
    "return": "sich die Wurst vom Brot nehmen lassen"
  },
  {
    "args": ["Bratwurst and Rostbratwurst is a sausage made from finely minced pork and beef and usually grilled and served with sweet German mustard and a piece of bread or hard roll. It can be sliced and made into Currywurst by slathering it in a catchup-curry sauce."],
    "return": "Bratwurst and Rostbratwurst is a Wurst made from finely minced pork and beef and usually grilled and served with sweet German mustard and a piece of bread or hard roll. It can be sliced and made into Currywurst by slathering it in a catchup-curry sauce."
  },
  {
    "args": ["Naem is a common way of preserving pork meat in several Southeast Asian countries, including Thailand, Laos, Cambodia and Vietnam"],
    "return": "Wurst is a common way of preserving pork meat in several Southeast Asian countries, including Thailand, Laos, Cambodia and Vietnam"
  },
  {
    "args": ["The chipper group over at Orangutan recently dropped another wheel sensation; the Moronga"],
    "return": "The chipper group over at Orangutan recently dropped another wheel sensation; the Wurst"
  }
]
```
## Credits

Found on Edabit: [Wurst Is Better](https://edabit.com/challenge/928sxbEt8gyZ5uBBt)
