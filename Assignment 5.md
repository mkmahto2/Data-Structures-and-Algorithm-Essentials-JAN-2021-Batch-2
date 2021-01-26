
## Question 1
Name 5 sorting algorithms, also write their time complexities(best, average, worst).
Both are calculated as the function of input size(n).

One important thing here is that in spite of these parameters the efficiency of an algorithm also depends upon the nature and size of the input. 

Following is a quick revision sheet that you may refer at last minute 

Algorithm	Time Complexity	 

+----------------+-------------+-------------+-------------+---+
|                | Best        | Average     |  Worst      |   |
+----------------+-------------+-------------+-------------+---+
| Selection Sort | Ω(n^2)      | θ(n^2)      | O(n^2)      |   |
+----------------+-------------+-------------+-------------+---+
| Bubble Sort    | Ω(n)        | θ(n^2)      | O(n^2)      |   |
+----------------+-------------+-------------+-------------+---+
| Insertion Sort | Ω(n)        | θ(n^2)      | O(n^2)      |   |
+----------------+-------------+-------------+-------------+---+
| Heap Sort      | Ω(n log(n)) | θ(n log(n)) | O(n log(n)) |   |
+----------------+-------------+-------------+-------------+---+
| Quick Sort     | Ω(n log(n)) | θ(n log(n)) | O(n^2)      |   |
+----------------+-------------+-------------+-------------+---+
| Merge Sort     | Ω(n log(n)) | θ(n log(n)) | O(n log(n)) |   |
+----------------+-------------+-------------+-------------+---+
| Bucket Sort    | Ω(n+k)      | θ(n+k)      | O(n^2)      |   |
+----------------+-------------+-------------+-------------+---+
| Radix Sort     | Ω(nk)       | θ(nk)       | O(nk)       |   |
+----------------+-------------+-------------+-------------+---+



	 
	 
 

## Question 2
Implement selection sort algorithm using Python.
~~~
def selectionSort(nlist):
   for fillslot in range(len(nlist)-1,0,-1):
       maxpos=0
       for location in range(1,fillslot+1):
           if nlist[location]>nlist[maxpos]:
               maxpos = location

       temp = nlist[fillslot]
       nlist[fillslot] = nlist[maxpos]
       nlist[maxpos] = temp

nlist = [14,46,43,27,57,41,45,21,70]
selectionSort(nlist)
print(nlist)

~~~

## Question 3
Implement pop operation of the stack
## Question 4
Implement dequeue operation of the queue
