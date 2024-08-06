# Python Lesson 6: Magic Spells (Functions)

## Let's Get Ready!
Remember our special coding playground? [Click here to open it](https://www.programiz.com/python-programming/online-compiler/)

## Today's Magical Adventure
After our journey, you'll be able to:
1. Understand what magic spells (functions) are and why they're super helpful
2. Create your own simple spells
3. Use spells with special ingredients (parameters)

## Part 1: What are Magic Spells?

Imagine you're a wizard in a magical world. Magic spells are like your special powers that you can use again and again. In Python, we call these spells "functions". They help us do amazing things with just a few words!

## Part 2: Creating Simple Spells

Let's learn how to create a simple spell:

```python
def say_hello():
    print("Hello, magical friend!")

# Use your spell
say_hello()
```

This is like writing a spell in your spell book and then using it!

### Your Magical Task:
1. Create a spell called `sing_chorus()`. Inside the spell, use `print()` to write out your favorite line from a magical song.
2. After creating your spell, call it three times to sing the magical chorus!

## Part 3: Spells with Special Ingredients

We can make our spells even more powerful by adding special ingredients. In Python, we call these "parameters":

```python
def greet(wizard_name):
    print("Greetings, " + wizard_name + "!")

# Use your spell
greet("Merlin")
greet("Gandalf")
```

### Your Magical Task:
1. Create a spell called `cast_spell(magic_word)`. Inside the spell, use `print()` to say "Abracadabra! I cast " followed by the `magic_word`.
2. After creating your spell, call it three times with different magic words, like "fireball", "invisibility", and "flying"!

## Let's Create: A Magical Pet Companion

Now, let's use our new spell-casting skills to create a program that helps us take care of a magical pet! Follow these steps:

1. First, let's create a spell to feed our pet:
   ```python
   def feed_pet(pet_name):
       # Use print() to say that pet_name is eating something yummy!
   ```

2. Next, create a spell to play with our pet:
   ```python
   def play_with_pet(pet_name):
       # Use print() to describe how you're playing with pet_name
   ```

3. Now, let's make a spell for pet sounds:
   ```python
   def pet_sounds(pet_name, sound):
       # Use print() to make pet_name say the sound
   ```

4. Time to use our spells! Start by asking for the pet's name:
   ```python
   pet_name = input("What's your magical pet's name? ")
   ```

5. Use your `feed_pet()` spell with the pet's name.

6. Use your `play_with_pet()` spell with the pet's name.

7. Ask what sound the pet makes:
   ```python
   pet_sound = input("What sound does " + pet_name + " make? ")
   ```

8. Use your `pet_sounds()` spell with the pet's name and sound.

### Extra Magic:
Can you add a new spell called `pet_sleep(pet_name)` to make your pet go to sleep? What would it print?

## Wonderful Work, Young Wizard!

You've learned how to create and use magical spells (functions) in Python! These spells help us organize our magical code and make it easy to do amazing things over and over. Keep practicing your magic and have fun with your new Python powers!
