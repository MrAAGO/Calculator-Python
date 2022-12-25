# Calculator-Python

# Function to perform the desired operation
def calculate(num1, num2, operator):
    if operator == "+":
        return num1 + num2
    elif operator == "-":
        return num1 - num2
    elif operator == "*":
        return num1 * num2
    elif operator == "/":
        return num1 / num2

# Main program
while True:
    # Get user input
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    operator = input("Enter operator (+, -, *, /): ")

    # Perform calculation and print result
    result = calculate(num1, num2, operator)
    print("Result:", result)

    # Prompt user to continue or exit
    cont = input("Do you want to perform another calculation? (y/n): ")
    if cont.lower() != "y":
        break
