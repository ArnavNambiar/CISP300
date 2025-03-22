# Lab 7-3 The Dice Game
# Programmer: Arnav Nambiar
# Date: 22 March 2025
# Description: This program simulates a dice game between two players.

import random  # imports the random library


# this function gets the players names
def inputNames(playerOne, playerTwo):
    playerOne = input("Enter Player One's name: ")  # Prompts for Player One's name
    playerTwo = input("Enter Player Two's name: ")  # Prompts for Player Two's name
    return playerOne, playerTwo  # Returns both player names


# this function will get the random values
def rollDice(p1number, p2number, playerOne, playerTwo, winnerName):
    p1number = random.randint(1, 6)  # Generates a random number between 1 and 6 for Player One
    p2number = random.randint(1, 6)  # Generates a random number between 1 and 6 for Player Two

    print(playerOne + " rolled a " + str(p1number))  # Displays Player One's roll
    print(playerTwo + " rolled a " + str(p2number))  # Displays Player Two's roll

    if p1number > p2number:  # checks if Player One's roll is greater than Player Two's roll
        winnerName = playerOne  # If true, Player One is the winner
    elif p2number > p1number:  # Otherwise, checks if Player Two's roll is greater than Player One's roll
        winnerName = playerTwo  # If true, Player Two is the winner
    else:
        winnerName = "TIE"  # If both rolls are equal, it's a tie

    return winnerName  # Returns the name of the winner


# this function displays the winner
def displayInfo(winnerName):
    if winnerName == "TIE":  # Checks if the game was a tie
        print("The game was a " + winnerName)  # If true, prints that the game was a tie
    else:
        print("The winner is " + winnerName)  # Otherwise, prints the name of the winner


# the main function
def main():
    print()

    # initialize variables
    endProgram = 'no'  # Initializes the endProgram variable to 'no' to start the game
    playerOne = 'NO NAME'  # Initializes playerOne's name to 'NO NAME'
    playerTwo = 'NO NAME'  # Initializes playerTwo's name to 'NO NAME'

    # call to inputNames
    playerOne, playerTwo = inputNames(playerOne, playerTwo)  # Calls the inputNames function to get player names

    # while loop to run program again
    while endProgram == 'no':

        # populate variables
        winnersName = 'NO NAME'  # Initializes the winner's name to 'NO NAME'
        p1number = 0  # Initializes Player One's number to 0
        p2number = 0  # Initializes Player Two's number to 0

        # call to rollDice
        winnersName = rollDice(p1number, p2number, playerOne, playerTwo,
                                  winnersName)  # Calls the rollDice function to determine the winner

        # call to displayInfo
        displayInfo(winnersName)  # Calls the displayInfo function to display the winner

        endProgram = input('Do you want to end program? (yes/no): ')  # Asks the user if they want to end the program


# calls main
main()
