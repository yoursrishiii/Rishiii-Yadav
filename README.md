1. Write a function employee_details(name, age, department) that prints employee information using keyword arguments and default argument department='CSE'. Call the function with arguments in different orders.

def employee_details(name, age, department='CSE'):
    print("Employee Name:", name)
    print("Age:", age)
    print("Department:", department)
    print("----------------------")

employee_details("Rishi", 20, "IT")
employee_details(age=22, name="Aman", department="ECE")
employee_details(name="Neha", age=21)
employee_details(age=25, name="Rahul")


2. Implement recursive function for finding factorial of a number.

def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))


3. Write a function filter_even_square(numbers) that takes a list of integers and returns a new list containing the squares of only even numbers using list comprehension.

def filter_even_square(numbers):
    return [x**2 for x in numbers if x % 2 == 0]

nums = [1, 2, 3, 4, 5, 6]
print(filter_even_square(nums))


4. Create a string and show string slicing, replication, concatenation and replacement.

s = "Hello World"

print(s[0:5])
print(s[::-1])

print(s * 2)

s2 = " Python"
print(s + s2)

print(s.replace("World", "Rishi"))
