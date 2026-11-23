# interactive-calculator-and-unit-converter

# PROJECT 01: INTERACTIVE CALCULATOR & UNIT CONVERTER

# Function 1: Arithmetic Calculator
def calculator():
    print("\n--- ARITHMETIC CALCULATOR ---")

    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    print("\n1. Addition (+)")
    print("2. Subtraction (-)")
    print("3. Multiplication (*)")
    print("4. Division (/)")

    choice = input("Choose an operation: ")

    if choice == "1":
        print("Result:", num1 + num2)

    elif choice == "2":
        print("Result:", num1 - num2)

    elif choice == "3":
        print("Result:", num1 * num2)

    elif choice == "4":
        if num2 != 0:
            print("Result:", num1 / num2)
        else:
            print("Error! Division by zero is not allowed.")

    else:
        print("Invalid operation!")


# Function 2: Currency Converter
def currency_converter():
    print("\n--- CURRENCY CONVERTER ---")

    amount = float(input("Enter amount in INR: "))

    print("1. INR to USD")
    print("2. INR to EUR")
    print("3. USD to INR")
    print("4. EUR to INR")

    choice = input("Choose conversion: ")

    # Illustrative rates only; update with current rates
    if choice == "1":
        print("USD:", amount / 85)

    elif choice == "2":
        print("EUR:", amount / 99)

    elif choice == "3":
        print("INR:", amount * 85)

    elif choice == "4":
        print("INR:", amount * 99)

    else:
        print("Invalid choice!")


# Function 3: Unit Converter
def unit_converter():
    print("\n--- UNIT CONVERTER ---")

    print("1. Kilometer to Meter")
    print("2. Meter to Kilometer")
    print("3. Kilogram to Gram")
    print("4. Gram to Kilogram")
    print("5. Celsius to Fahrenheit")
    print("6. Fahrenheit to Celsius")

    choice = input("Choose conversion: ")

    value = float(input("Enter value: "))

    if choice == "1":
        print("Meters:", value * 1000)

    elif choice == "2":
        print("Kilometers:", value / 1000)

    elif choice == "3":
        print("Grams:", value * 1000)

    elif choice == "4":
        print("Kilograms:", value / 1000)

    elif choice == "5":
        print("Fahrenheit:", (value * 9/5) + 32)

    elif choice == "6":
        print("Celsius:", (value - 32) * 5/9)

    else:
        print("Invalid choice!")


# Main Program
while True:

    print("\n================================")
    print(" INTERACTIVE CALCULATOR")
    print("================================")

    print("1. Arithmetic Calculator")
    print("2. Currency Converter")
    print("3. Unit Converter")
    print("4. Exit")

    main_choice = input("\nEnter your choice: ")

    if main_choice == "1":
        calculator()

    elif main_choice == "2":
        currency_converter()

    elif main_choice == "3":
        unit_converter()

    elif main_choice == "4":
        print("Thank you for using the program!")
        break

    else:
        print("Invalid choice! Please try again.")
