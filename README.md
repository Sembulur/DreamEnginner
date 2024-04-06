# DreamEnginner
import random

def guess_number():
    number = random.randint(1, 100)
    attempts = 0

    print("Welcome to the Guess the Number Game!")
    print("I have chosen a number between 1 and 100. Can you guess it?")

    while True:
        guess = int(input("Enter your guess: "))
        attempts += 1

        if guess < number:
            print("Too low! Try again.")
        elif guess > number:
            print("Too high! Try again.")
        else:
            print(f"Congratulations! You've guessed the number {number} correctly in {attempts} attempts.")
            break

if __name__ == "__main__":
    guess_number()
