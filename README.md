# calculator1234
import math

def add():
    x = float(input("Enter the first number: "))
    y = float(input("Enter the second number: "))
    return x + y

def sub():
    x = float(input("Enter the first number: "))
    y = float(input("Enter the second number: "))
    return x - y

def mul():
    x = float(input("Enter the first number: "))
    y = float(input("Enter the second number: "))
    return x * y

def div():
    x = float(input("Enter the first number: "))
    y = float(input("Enter the second number: "))
    if y == 0:
        return "Error: Division by zero"
    else:
        return x / y

def square_root():
    x = float(input("Enter a number: "))
    return math.sqrt(x)

def cube_root():
    x = float(input("Enter a number: "))
    return x ** (1/3)

def power():
    x = float(input("Enter the base number: "))
    y = float(input("Enter the exponent: "))
    return x ** y

def logarithm():
    x = float(input("Enter a number: "))
    if x <= 0:
        return "Error: Logarithm is not defined for non-positive numbers."
    else:
        return math.log(x)

while True:
    print("Welcome to your personal calculator")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Square Root")
    print("6. Cube Root")
    print("7. Power")
    print("8. Logarithm")
    print("9. Exit")

    choice = int(input("Enter your choice: "))
    
    if choice == 1:
        result = add()
        print(f"Result: {result}")
    elif choice == 2:
        result = sub()
        print(f"Result: {result}")
    elif choice == 3:
        result = mul()
        print(f"Result: {result}")
    elif choice == 4:
        result = div()
        print(f"Result: {result}")
    elif choice == 5:
        result = square_root()
        print(f"Result: {result}")
    elif choice == 6:
        result = cube_root()
        print(f"Result: {result}")
    elif choice == 7:
        result = power()
        print(f"Result: {result}")
    elif choice == 8:
        result = logarithm()
        print(f"Result: {result}")
    elif choice == 9:
        print("Exiting the calculator. Goodbye!")
        break  # Exit the while loop
    else:
        print("Enter a valid option.")
