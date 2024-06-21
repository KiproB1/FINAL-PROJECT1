# FINAL-PROJECT1
Python 
# Mad Libs Generator
nouns = ["dog", "cat", "house"]
verbs = ["run", "jump", "sleep"]
adjectives = ["happy", "sad", "tired"]

print("Let's play Mad Libs!")

noun = input("Enter a noun: ")
verb = input("Enter a verb: ")
adjective = input("Enter an adjective: ")

story = f"The {adjective} {noun} likes to {verb} all day long."

print(story)
Let's play Mad Libs!
Enter a noun: dog
Enter a verb: jump
Enter an adjective: happy

The happy dog likes to jump all day long.
# Number Guessing Game
import random

secret_number = random.randint(1, 10)
guesses = 3

while guesses > 0:
  guess = int(input("Guess a number between 1 and 10: "))
  guesses -= 1

  if guess == secret_number:
    print("You guessed it!")
    break
  elif guess > secret_number:
    print("Too high! Guess again.")
  else:
    print("Too low! Guess again.")

if guesses == 0:
  print("You ran out of guesses. The number was", secret_number)
Guess a number between 1 and 10: 5
Too low! Guess again.
Guess a number between 1 and 10: 8
Too high! Guess again.
Guess a number between 1 and 10: 7
You guessed it!
