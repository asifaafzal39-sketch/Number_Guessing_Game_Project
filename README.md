# Number_Guessing_Game_Project

import random

# Computer picks a random number between 1 and 50
secret_number = random.randint(1, 50)

print("Welcome to the Guessing Game!")
print("I have chosen a number between 1 and 50.")

while True:
    # Take input from user
    guess = int(input("Enter your guess: "))

    # Check the guess
    if guess > secret_number:
        print("Too high! Try again.")
    elif guess < secret_number:
        print("Too low! Try again.")
    else:
        print("Congratulations! You guessed the correct number!")
        break  # Exit the loop when correct
