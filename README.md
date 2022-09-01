
#Rock Paper Scissors Game
#By Suavecito

import random

options = ["rock","paper","scissors"]



#Main function of game
def main():

    #get user input and random computer choice
    user = input ("rock, paper, or scissors\n\nyour choice: ")
    pc = random.choice(options)
    print ("PC's Choice: "+pc)
    #get rid of white space from user
    user = user.strip()

    #compare user input to computer response and get results
    if user.lower() == "scissors":
        if pc == "scissors":
            print ("\nTie, you still suck.")
        if pc == "rock":
            print ("\nLoser, thats why no one loves you.")
        if pc == "paper":
            print ("\nWinner winner chicken dinner!")

    if user.lower() == "rock":
        if pc == "rock":
            print ("\nTie, you still suck.")
        if pc == "paper":
            print ("\nLoser, thats why no one loves you.")
        if pc == "scissors":
            print ("\nWinner winner chicken dinner!")

    if user.lower() == "paper":
        if pc == "paper":
            print ("\nTie, you still suck.")
        if pc == "scissors":
            print ("\nLoser, thats why no one loves you.")
        if pc == "rock":
            print ("\nWinner winner chicken dinner!")
    user = input ("\nDo you want to play again?\nY/N:")
    
    #Continue the script or not
    if user.lower() == "y" or "yes":
        main()
    else:
        exit()


if __name__ == '__main__':
    main()
