# Number_Guessing_Game_In_Python

import random

# Generate a random number between 1 and 100
ran_number = random.randint(1, 100)

attempts = 0

print("Welcome to the Number Guessing Game!")
print("Guess a number between 1 and 100.")

while True:
    guess = int(input("Enter your guess: "))
    attempts += 1
    if guess < ran_number:
        print("Too low! Try again.")
    elif guess > ran_number:
        print("Too high! Try again.")
    else:
        print("Congratulations! You guessed the correct number.")
        print("Number of attempts:", attempts)
        break
