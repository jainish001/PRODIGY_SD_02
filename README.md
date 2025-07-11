# PRODIGY_SD_02

import random


n = random.randint(1, 100)

a = -1  
guesses = 1 

print("Welcome to the Guessing Game!")
print("Guess the number between 1 and 100")


while a != n:
    a = int(input("Guess the number: "))

    if a > n:
        print("Too high! Try a lower number.")
        guesses += 1
    elif a < n:
        print("Too low! Try a higher number.")
        guesses += 1


print(f" You guessed the number {n} correctly in {guesses} attempts!")
