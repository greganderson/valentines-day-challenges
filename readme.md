# Valentine's Day Challenges

Welcome to the Valentine's Day Challenges! We've got a list of challenges here that need solving in order to have
a good Valentine's Day. However, these challenges can't just be solved like normal! They can only be solved on paper,
with the only tool to help being the python interactive shell! That said, I know you're up to the challenge, and that
you can save Valentine's Day. Good luck!


## Challenges

Remember, these challenges can only be solved on paper, but you _can_ use the python interactive shell. Unfortunately,
ChatGPT, Copilot, and VS Code have all conspired to ruin Valentine's Day, so you cannot use them to help you. All other
IDE's like Pycharm have all joined in the efforts to destroy everyone's happiness.


### He/She Loves Me

Write a function that takes the number of petals on a flower, then plucks petals to determine if someone loves you.
Each time a petal is plucked, you say "He loves me" or "He loves me not" (could also be used with "She") then at the
end when you've determined which it is, return whether or not the person loves you.

Example:

```python
she_loves_me = pluck_petals(30)
# prints "She loves me" and "She loves me not" a bunch of times
if she_loves_me:
    print("She loves me!")
else:
    print("She doesn't love me :(")
```


### Number of Valentines

In elementary school, valentines are sometimes exchanged. Given a `Student`, determine whether or not they have enough
valentines to be happy. You'll find the `Student` class in the `number_of_valentines` folder.

Example:

```python
greg = Student(num_valentines=9)

# You determine how many is enough
enough = has_enough_valentines(greg)

if enough:
    print(f"{greg.name} had enough valentines!")
else:
    print(f"{greg.name} didn't have enough valentines :(")
```


### Love Letter

Passing love letters is a nice thing to do. Create a `Letter` class that has `to`, `from`, and `contents` member variables.
Create a `Person` class that has a `name`, and a list of `Letter`'s, and has a method that lets the `Person` Write
a `Letter` to another `Person`, a method that receives a `Letter`, and a method that prints out all the `Letter`'s a `Person`
has.

Example:

```python
greg = Person(name="Greg")
kylie = Person(name="Kylie")

greg.print_letters()
# prints nothing, he doesn't have any letters

letter_to_kylie = Letter(to=kylie, contents="Dear Kylie, you are the best!")
greg.write_letter(to=kylie, letter=letter_to_kylie)

kylie.print_letters()
# -> "Dear Kylie, you are the best!"
```


### Flower Bouquet Cost Calculator

Giving flowers on Valentine's Day is tradition, guys have to do it. It's also tradition that guys get in trouble when
they forget. Create a function that takes in a list of `Flower`'s, then calculates the cost of the bouquet. The `Flower`
class can be found in the `bouquet_calculator` folder.

Example:

```python
bouquet = [Flower.ROSE, Flower.EDELWEISS, Flower.LILY]
cost = calculate_bouquet_cost(bouquet)
print(f"The cost is ${cost}")
# prints $27.99
```


### Compliment Generator

Sometimes you've gotta come up with compliments on the fly. Lets make a function that can help! Create a function that
randomly chooses from a random list of compliments and returns it.

Example:

```python
compliment = get_random_compliment()
print(compliment)
# "My you look dashing today!"
```
