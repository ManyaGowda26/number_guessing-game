# number_guessing-game

import random

number = random.randint(1, 100)
attempts = 0

print("Welcome to the Number Guessing Game!")
print("Guess a number between 1 and 100")

while True:
    guess = int(input("Enter your guess: "))
    attempts += 1

    if guess < number:
        print("Too low! Try again.")
    elif guess > number:
        print("Too high! Try again.")
    else:
        print("Congratulations! You guessed it!")
        print("Number of attempts:", attempts)
        break


Output:

Welcome to the Number Guessing Game!
Guess a number between 1 and 100

Enter your guess: 30
Too low! Try again.

Enter your guess: 70
Too high! Try again.

Enter your guess: 50
Congratulations! You guessed it!
Number of attempts: 3
