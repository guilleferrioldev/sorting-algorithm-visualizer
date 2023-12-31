# sorting-algorithm-visualizer
Python sorting algorithm visualizer.

In this project we have used python language because of it's extensive librarires and easy syntax. By using the pygame library we will visualize all the sorting algorithm. By looking at the graph how data is sorted we will analyze which sorting technique perform best under a specificc situatiion. Before writing the prgoram we will setup the Envirement for pygame and we will Install the pakages. The Gui will be provided by pygame. After installation we are good to run the python program to visualize sorting algorithms on the screen. 
1. Install Pygame
2. Include library in the program
3. Code for all the sorting Algorithm 
4. Run the above python file in any of your faviroite IDE and see the magic ;)
5. You will see visualization of all sorting Algorithms

### Install requirements 

 
```
python -r requirements.txt

```


### Run 

Open the app folder and run the following command

```
python main.py

```

### About the GUI and How it works
When you will run the above code. A screen will pop up.
This screen contain name of all nine Algorithms , Set and resset button and also it provides you option to select Ascecending or Desecending.
For example if you want to Select Bubble Sort You havve to Press (B) and For Ascending (A) and then press SPACE.
Now visualization will be start for the Random Data.


### Pictures 

![pic](./picture/sorting.png)

![radix](./picture/radix.png)

## Bubble sort 
Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in the wrong order. This algorithm is not suitable for large data sets as its average and worst-case time complexity is quite high.


## selection sort
The selection sort algorithm sorts an array by repeatedly finding the minimum element (considering ascending order) from the unsorted part and putting it at the beginning. 
The algorithm maintains two subarrays in a given array.

The subarray which already sorted. 
The remaining subarray was unsorted.


## Insertion sort 
Insertion sort is a simple sorting algorithm that works similar to the way you sort playing cards in your hands. The array is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part.

Characteristics of Insertion Sort:
This algorithm is one of the simplest algorithm with simple implementation
Basically, Insertion sort is efficient for small data values
Insertion sort is adaptive in nature, i.e. it is appropriate for data sets which are already partially sorted.


## Merge Sort
The Merge Sort algorithm is a sorting algorithm that is based on the Divide and Conquer paradigm. In this algorithm, the array is initially divided into two equal halves and then they are combined in a sorted manner.
Merge Sort Working Process:
Think of it as a recursive algorithm continuously splits the array in half until it cannot be further divided. This means that if the array becomes empty or has only one element left, the dividing will stop, i.e. it is the base case to stop the recursion. If the array has multiple elements, split the array into halves and recursively invoke the merge sort on each of the halves. Finally, when both halves are sorted, the merge operation is applied. Merge operation is the process of taking two smaller sorted arrays and combining them to eventually make a larger one.


## Quicksort
QuickSort is a Divide and Conquer algorithm. It picks an element as a pivot and partitions the given array around the picked pivot. There are many different versions of quickSort that pick pivot in different ways. 
Always pick the first element as a pivot.
Always pick the last element as a pivot (implemented below)
Pick a random element as a pivot.
Pick median as the pivot.
The key process in quickSort is a partition(). The target of partitions is, given an array and an element x of an array as the pivot, put x at its correct position in a sorted array and put all smaller elements (smaller than x) before x, and put all greater elements (greater than x) after x. All this should be done in linear time.


## Heap Sort
Heap sort is a comparison-based sorting technique based on Binary Heap data structure. It is similar to the selection sort where we first find the minimum element and place the minimum element at the beginning. Repeat the same process for the remaining elements.
Heap sort is an in-place algorithm. 
Its typical implementation is not stable, but can be made stable (See this)
Typically 2-3 times slower than well-implemented QuickSort.  The reason for slowness is a lack of locality of reference.


## Radix Sort
The lower bound for the Comparison based sorting algorithm (Merge Sort, Heap Sort, Quick-Sort .. etc) is Ω(nLogn), i.e., they cannot do better than nLogn. Counting sort is a linear time sorting algorithm that sort in O(n+k) time when elements are in the range from 1 to k.

What if the elements are in the range from 1 to n2? 
We can’t use counting sort because counting sort will take O(n2) which is worse than comparison-based sorting algorithms. Can we sort such an array in linear time? 
Radix Sort is the answer. The idea of Radix Sort is to do digit by digit sort starting from least significant digit to most significant digit. Radix sort uses counting sort as a subroutine to sort.


## Bucket Sort 
Bucket sort is mainly useful when input is uniformly distributed over a range. For example, consider the following problem. 
Sort a large set of floating point numbers which are in range from 0.0 to 1.0 and are uniformly distributed across the range. How do we sort the numbers efficiently?
A simple way is to apply a comparison based sorting algorithm. The lower bound for Comparison based sorting algorithm (Merge Sort, Heap Sort, Quick-Sort .. etc) is Ω(n Log n), i.e., they cannot do better than nLogn. 
Can we sort the array in linear time? Counting sort can not be applied here as we use keys as index in counting sort. Here keys are floating point numbers.  
The idea is to use bucket sort. Following is bucket algorithm.


## Counting sort
Counting sort is a sorting technique based on keys between a specific range. It works by counting the number of objects having distinct key values (kind of hashing). Then do some arithmetic to calculate the position of each object in the output sequence. 
Characteristics of counting sort:
Counting sort makes assumptions about the data, for example, it assumes that values are going to be in the range of 0 to 10 or 10 – 99 etc, Some other assumptions counting sort makes are input data will be all real numbers.
Like other algorithms this sorting algorithm is not a comparison-based algorithm, it hashes the value in a temporary count array and uses them for sorting.
It uses a temporary array making it a non In Place algorithm.


# Links and Refrences 
https://youtu.be/twRidO-_vqQ

https://www.geeksforgeeks.org/

https://stackoverflow.com/

https://docs.python.org/3/

https://www.pygame.org/docs/
