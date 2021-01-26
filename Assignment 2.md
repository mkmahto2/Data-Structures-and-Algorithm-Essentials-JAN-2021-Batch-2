
## Question 1
Write a Python program to print even numbers in a list.
Sample:
Input: list1 = [12, 3, 55, 6, 144]
Output: [12, 6, 144]
Input: list2 = [2, 10, 9, 37]
Output: [2, 10]
~~~
list1 = [10, 21, 4, 45, 66, 93] 

  
# iterating each number in list 

for num in list1: 

      

    # checking condition 

    if num % 2 == 0: 

       print(num, end = " ") 

~~~
## Question 2
Write a program to print the following pattern
1
22
333
4444
55555

~~~
rows = 6
for num in range(rows):
    for i in range(num):
        print(num, end=" ")  # print number
    # line after each row to display pattern correctly
    print(" ")

~~~
