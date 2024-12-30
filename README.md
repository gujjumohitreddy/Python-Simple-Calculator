#Creating a simple Python calculator is a great way for beginners to practice programming. Below is a basic example of a Python calculator that can perform addition, subtraction, multiplication, and division:

#Simple Python Calculator

Function for addition
def add(x, y):
    return x + y

Function for subtraction
def subtract(x, y):
    return x - y

Function for multiplication
def multiply(x, y):
    return x * y

Function for division
def divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Error! Division by zero."

Display menu
def menu():
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")

Main program loop
while True:
    menu()

    # Take input from the user
    choice = input("Enter choice (1/2/3/4): ")

    # Check if the user wants to exit
    if choice == '5':
        print("Exiting the calculator.")
        break

    # Check if the user entered a valid choice
    if choice in ['1', '2', '3', '4']:
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        # Perform the operation based on user choice
        if choice == '1':
            print(f"{num1} + {num2} = {add(num1, num2)}")
