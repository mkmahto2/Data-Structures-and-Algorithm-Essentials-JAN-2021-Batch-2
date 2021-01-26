
## Question 1
Implement deletion operation from the end of the linked list and Insertion operation from the
beginning of the linked list.


## Question 2
Implement binary search using python language.
(Write a function which returns the index of x in given array arr if present, else returns -1)
~~~

# Iterative Binary Search Function 
# It returns index of x in given array arr if present, 
# else returns -1 

def binary_search(arr, x): 

    low = 0

    high = len(arr) - 1

    mid = 0

  

    while low <= high: 

  

        mid = (high + low) // 2

  

        # Check if x is present at mid 

        if arr[mid] < x: 

            low = mid + 1

  

        # If x is greater, ignore left half 

        elif arr[mid] > x: 

            high = mid - 1

  

        # If x is smaller, ignore right half 

        else: 

            return mid 

  

    # If we reach here, then the element was not present 

    return -1

  

  
# Test array 

arr = [ 2, 3, 4, 10, 40 ] 

x = 10

  
# Function call 

result = binary_search(arr, x) 
~~~
## Question 3
Write a Python program to find the middle of a linked list.
~~~
class Node:
    def __init__(self, data):
       self.data = data
       self.next = None
 
 
class LinkedList:
    def __init__(self):
        self.head = None
        self.last_node = None
 
    def append(self, data):
        if self.last_node is None:
            self.head = Node(data)
            self.last_node = self.head
        else:
            self.last_node.next = Node(data)
            self.last_node = self.last_node.next
 
 
def print_middle(llist):
    current = llist.head
    length = 0
    while current:
        current = current.next
        length = length + 1
 
    current = llist.head
    for i in range((length - 1)//2):
        current = current.next
 
    if current:
        if length % 2 == 0:
            print('The two middle elements are {} and {}.'
                .format(current.data, current.next.data))
        else:
            print('The middle element is {}.'.format(current.data))
    else:
        print('The list is empty.')
 
 
a_llist = LinkedList()
 
data_list = input('Please enter the elements in the linked list: ').split()
for data in data_list:
    a_llist.append(int(data))
 
print_middle(a_llist)

~~~
