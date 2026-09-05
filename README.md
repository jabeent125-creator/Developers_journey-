# Developers_journey-
"Building the foundation: Turning logic into solutions and ideas into software."
while True:
    print("\nPython Calculator")
    print("Enter 'q' to quit")

    first = input("Enter first number: ")

    if first.lower() == "q":
        print("Goodbye!")
        break

    operator = input("Enter operator (+, -, *, /): ")

    second = input("Enter second number: ")

    try:
        num1 = float(first)
        num2 = float(second)

        if operator == "+":
            result = num1 + num2
        elif operator == "-":
            result = num1 - num2
        elif operator == "*":
            result = num1 * num2
        elif operator == "/":
            if num2 == 0:
                print("Error: Cannot divide by zero.")
                continue
            result = num1 / num2
        else:
            print("Invalid operator.")
            continue

        print("Result:", result)

    except ValueError:
        print("Please enter valid numbers.")