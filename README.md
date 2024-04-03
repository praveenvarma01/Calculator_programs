# Calculator_programs
def calculator():
    # Prompt the user for two numbers
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))

    # Prompt the user for the operation choice
    operation = input("Enter the operation (+, -, *, /): ")

    # Perform the calculation based on the user's choice
    if operation == "+":
        result = num1 + num2
    elif operation == "-":
        result = num1 - num2
    elif operation == "*":
        result = num1 * num2
    elif operation == "/":
        if num2 != 0:
            result = num1 / num2
        else:
            print("Error: Division by zero is not allowed.")
            return
    else:
        print("Invalid operation. Please try again.")
        return

    # Display the result
    print(f"The result of {num1} {operation} {num2} is: {result}")

# Call the calculator function
calculator()
