#Arnav Nambiar
#22 March 2025
#7.4Lab

import random


# Function to get the student's name
def input_names():
 student_name = input("Enter Student Name: ")
 return student_name


# Function to generate two random numbers between 1 and 500
def get_numbers():
 number1 = random.randint(1, 500)
 number2 = random.randint(1, 500)
 return number1, number2


# Function to display the equation and get the student's answer
def get_answer(number1, number2):
 print("What is the answer to the following equation")
 print(number1)
 print("+")
 print(number2)
 answer = int(input("What is the sum: "))
 return answer


# Function to check if the answer is correct and update the score
def check_answer(number1, number2, answer, right):
 if answer == number1 + number2:
 print("Right")
 right += 1
 else:
 print("Wrong")
 return right


# Function to calculate the average score
def calculate_results(right):
 average_right = right / 10
 return average_right


# Function to display the student's information and results
def display_info(right, average_right, student_name):
 print("\nInformation for student:", student_name)
 print("The number right:", right)
 print("The average right is: {:.2f} or {:.1f}%".format(average_right, average_right * 100))


# Main function to run the math quiz program
def main():
 # Declare and initialize variables
 counter = 0
 student_name = "NO NAME"
 average_right = 0.0
 right = 0
 number1 = 0
 number2 = 0
 answer = 0


 # Get the student's name
 student_name = input_names()


 # Loop to ask 10 math questions
 while counter < 10:
 # Generate two random numbers
 number1, number2 = get_numbers()


 # Get the student's answer
 answer = get_answer(number1, number2)


 # Check if the answer is correct and update the score
 right = check_answer(number1, number2, answer, right)


 # Increment the counter
 counter += 1


 # Calculate the average score
 average_right = calculate_results(right)


 # Display the student's information and results
 display_info(right, average_right, student_name)


# Call the main function to start the program
if __name__ == "__main__":
 main()
