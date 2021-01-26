
## Question 1
Write a Python program to add two numbers using class and object.
(Take both numbers as input from the user)
~~~
class Test:

    def findsum(self, a, b):
        s = a + b
        return s


a = int(input("Enter first number:"))
b = int(input("Enter second number:"))

obj = Test()
s = obj.findsum(a, b)

print("Sum is:", s)
~~~
##Question 2
Define a function swap that should swap two values and print the swapped variables outside the
swap function.

~~~
#Python program to swap two variables without using third variable
def swap(a, b):
    t = a
    a = b
    b = t
    return a, b

#getting input from the user
a = float(input("Enter the first number: "))
b = float(input("Enter the second number: "))

#calling the function
a, b = swap(a, b)

#printing the output
print("Swapped value of x is %d & y is %d" %(a,b))
~~~
