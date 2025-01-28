# Simple-calculator
Python Code: A calculator program written in Python

```
print("1 is for addition operation")
print("2 is for subtraction operation")
print("3 is for multiplication operation")
print("4 is for division operation")

try:
    operation = int(input("Enter the operation: "))
    
    if (operation in [1, 2, 3, 4]):
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))
        
        if operation == 1:
            result = num1 + num2
        elif operation == 2:
            result = num1 - num2
        elif operation == 3:
            result = num1 * num2
        elif operation == 4:
            if num2 == 0:
                print("Error: Division by zero is not allowed.")
            else:
                result = num1 / num2
        
        if operation != 4 or num2 != 0:
            print("The result of the operation is: {}".format(result))
    else:
        print("Entered choice is an invalid number.")
except ValueError:
    print("Error: Please enter a valid number.")

```
