#GuessTheNumberGame

Guess The number game was made to simply exercise

![GitHub commit activity](https://img.shields.io/github/commit-activity/w/Bogdan0255/Guess-the-number)

Followers

![GitHub followers](https://img.shields.io/github/followers/Bogdan0255?style=social)

## Usage



```python
import random

top_of_range = input("Type a number: ")

if top_of_range.isdigit():
    top_of_range = int(top_of_range)

    if top_of_range <= 0:
        print("Please type a number larger than 0 next time.")
        quit()
else:
    print("Please type a number next time.")
    quit()

random_number = random.randint(0, top_of_range)
guesses = 0

while True:
    guesses +=1
    user_guess = input("Make a guess: ")
    if user_guess.isdigit():
        user_guess = int(user_guess)
    else:
        print("Please type a number next time.")
        continue

    if user_guess == random_number:
        print("You got it correct!")
        break
    elif user_guess > random_number:
            print("You were above the number!")
    else:
            print("You were below the number!")

print("You got it in", guesses, "guesses")
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## About me
Python and technologies enthusiast
