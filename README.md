# PYTHON-NUMBER-GUESSING-GAME
This is the basic python Number Guessing game 


import random
number_to_guess = random.randint(1, 100)
number_of_attempt = 0
def guess_number():
   
    print("Welcome to the Number Guessing game !")
    print("I'm thinking of a number between 1 to 100")

    
while True:
    guess = input("enter the gussing number :")

    if guess.isdigit():
        guess = int(guess)
        number_of_attempt +=1

        if guess < number_to_guess:
            print("Too Low !! Try again.")
        elif guess > number_to_guess:
            print("Too Big!! Try again")
        else:
            print(f"YOU GUESSED THE NUMBER RIGHT !! , IN {number_of_attempt} attempts")
            break

    else:
        print("PLEASE ENTER THE VALID NUMBER!!")


if __name__ =="__main__":
    guess_number()
