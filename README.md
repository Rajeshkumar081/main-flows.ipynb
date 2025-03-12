# main-flows.ipynb


#The sum of Two Numbers

num1 = int(input("Enter the first number: "))
num2 = int(input("Enter the second number: "))

sum_result = num1 + num2
print("The sum of", num1, "and", num2, "is:", sum_result)

#even and odd
num = int(input("Enter a number: "))

if num % 2 == 0:
    print("Even")
else:
    print("Odd")

#Fibonacci Sequence
n = int(input("Enter the number of terms in the Fibonacci sequence: "))

fib_sequence = [0, 1]

for i in range(2, n):
    next_number = fib_sequence[-1] + fib_sequence[-2]
    fib_sequence.append(next_number)
print("Fibonacci sequence:")
print(fib_sequence[:n])


#Factorial Calculation

n = int(input("Enter a number: "))
factorial = 1
for i in range(1, n + 1):
    factorial *= i

print(f"The factorial of {n} is {factorial}")

#Reverse a String

input_string = input("Enter a string: ")
reversed_string = input_string[::-1]

print(f"The reversed string is: {reversed_string}")

#Palindrome
input_string = input("Enter a string: ")

is_palindrome = input_string == input_string[::-1]
print(f"Is the string a palindrome? {is_palindrome}")

#Leap Year Check

year = int(input("Enter a year: "))
if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print("True")  
else:
    print("False")

#Armstrong Number

n = int(input("Enter a number: "))
num_str = str(n)

num_digits = len(num_str)
sum_of_powers = sum(int(digit) ** num_digits for digit in num_str)
if sum_of_powers == n:
    print("True")
else:
    print("False")

