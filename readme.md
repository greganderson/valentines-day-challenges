# Valentine's Day Challenges

Welcome to the Valentine's Day Challenges! We've got a list of challenges here that need solving in order to have
a good Valentine's Day. However, these challenges can't just be solved like normal! They can only be solved on paper,
with the only tool to help being the python interactive shell! That said, I know you're up to the challenge, and that
you can save Valentine's Day. Good luck!


## Challenges

Remember, these challenges can only be solved on paper, but you _can_ use the python interactive shell. Unfortunately,
ChatGPT, Copilot, and VS Code have all conspired to ruin Valentine's Day, so you cannot use them to help you. All other
IDE's like Pycharm have all joined in the efforts to destroy everyone's happiness. Even vim, despite it's good-natured
heart, has decided nobody should be happy on Valentine's Day. Emacs, as always, wants everyone to be unhappy. No changes
there.

Another command you are able to use is `cat`, which when run on a file, prints out the contents. For example, doing this:

```bash
cat readme.md
```

would print out this entire file onto your screen. Super handy when you want to see the contents of one of the class
files!


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
valentines to be happy. You'll find the `Student` class in the `number_of_valentines` folder. How many valentines is
enough? That depends! Some people think you need 4-5, then you're good. In 3rd grade, some kids might think you need
at least 15. As an adult, maybe 1 is enough, so long as it is from the right person. So how many is enough? You decide!
Maybe it depends on the person asking 🤔

Example:

```python
greg = Student(name="Greg", num_valentines=9)

# You determine how many is enough
enough = has_enough_valentines(greg)

if enough:
    print(f"{greg.name} had enough valentines!")
else:
    print(f"{greg.name} didn't have enough valentines :(")
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


### Love Calculator

In middle school, sometimes kids will come up with ways to determine whether or not two people are compatible. Create
a function that takes two names and says how compatible they are on a scale of 1-10. You could use the number of
characters in the name, the number of similar characters, or any other metric you want!

Example:

```python
love_rating = calculate_love_compatibility("Greg", "Kylie")
print(love_rating)
# 8.0 because 4/5 is .8
```


### Love Letter

Passing love letters is a nice thing to do. Create a `Letter` class that has `to`, `from_name`, and `contents` member variables.
Create a `Person` class that has a `name`, and a list of `Letter`'s, and has a method that lets them write a `Letter`
to another `Person`, a method that receives a `Letter`, and a method that prints out all the `Letter`'s a `Person` has.

Example:

```python
greg = Person(name="Greg")
kylie = Person(name="Kylie")

greg.print_letters()
# prints nothing, he doesn't have any letters

greg.write_letter(to=kylie, contents="Dear Kylie, you are the best!")

kylie.print_letters()
# -> "Dear Kylie, you are the best!"
```


### Heart Generator

This challenge is a special one. Because of the outcomes of your function, vim has decided you can use it to write your
solution. Write a function that prints out a heart or a broken heart out of characters based on an input of whether or
not someone has a full heart ❤️, or a broken heart 💔.

Example:

```python
broken_heart = False
print_heart(broken_heart)
# ASCII art heart gets printed
```
