# Data structure and algorithm in c++

Data Structure can be defined as the group of data elements which provides an efficient way of storing and organising data in the computer so that it can be used efficiently. Some examples of Data Structures are arrays, Linked List, Stack, Queue, etc. Data Structures are widely used in almost every aspect of Computer Science i.e. Operating System, Compiler Design, Artifical intelligence, Graphics and many more.

Data Structures are the main part of many computer science algorithms as they enable the programmers to handle the data in an efficient way. It plays a vitle role in enhancing the performance of a software or a program as the main function of the software is to store and retrieve the user's data as fast as possible

# Basic Terminology:

Data structures are the building blocks of any program or the software. Choosing the appropriate data structure for a program is the most difficult task for a programmer. Following terminology is used as far as data structures are concerned

Data: Data can be defined as an elementary value or the collection of values, for example, student's name and its id are the data about the student.

Group Items: Data items which have subordinate data items are called Group item, for example, name of a student can have first name and the last name.

Record: Record can be defined as the collection of various data items, for example, if we talk about the student entity, then its name, address, course and marks can be grouped together to form the record for the student.

File: A File is a collection of various records of one type of entity, for example, if there are 60 employees in the class, then there will be 20 records in the related file where each record contains the data about each employee.

Attribute and Entity: An entity represents the class of certain objects. it contains various attributes. Each attribute represents the particular property of that entity.

Field: Field is a single elementary unit of information representing the attribute of an entity.

# Need of Data Structures

As applications are getting complexed and amount of data is increasing day by day, there may arrise the following problems:

Processor speed: To handle very large amout of data, high speed processing is required, but as the data is growing day by day to the billions of files per entity, processor may fail to deal with that much amount of data.

Data Search: Consider an inventory size of 106 items in a store, If our application needs to search for a particular item, it needs to traverse 106 items every time, results in slowing down the search process.

Multiple requests: If thousands of users are searching the data simultaneously on a web server, then there are the chances that a very large server can be failed during that process

in order to solve the above problems, data structures are used. Data is organized to form a data structure in such a way that all items are not required to be searched and required data can be searched instantly.

# Advantages of Data Structures:

Efficiency: Efficiency of a program depends upon the choice of data structures. For example: suppose, we have some data and we need to perform the search for a perticular record. In that case, if we organize our data in an array, we will have to search sequentially element by element. hence, using array may not be very efficient here. There are better data structures which can make the search process efficient like ordered array, binary search tree or hash tables.

Reusability: Data structures are reusable, i.e. once we have implemented a particular data structure, we can use it at any other place. Implementation of data structures can be compiled into libraries which can be used by different clients.

Abstraction: Data structure is specified by the ADT which provides a level of abstraction. The client program uses the data structure through interface only, without getting into the implementation details.

# Algorithm:

An algorithm is a procedure having well defined steps for solving a particular problem. Algorithm is finite set of logic or instructions, written in order for accomplish the certain predefined task. It is not the complete program or code, it is just a solution (logic) of a problem, which can be represented either as an informal description using a Flowchart or Pseudo code.

The major categories of algorithms are given below:

Sort: Algorithm developed for sorting the items in certain order.

Search: Algorithm developed for searching the items inside a data structure.

Delete: Algorithm developed for deleting the existing element from the data structure.

Insert: Algorithm developed for inserting an item inside a data structure.

Update: Algorithm developed for updating the existing element inside a data structure.


The performance of algorithm is measured on the basis of following properties:

Time complexity: It is a way of representing the amount of time needed by a program to run to the completion.

Space complexity: It is the amount of memory space required by an algorithm, during a course of its execution. Space complexity is required in situations when limited memory is available and for the multi user system.

Asymptotic Analysis
In mathematical analysis, asymptotic analysis of algorithm is a method of defining the mathematical boundation of its run-time performance. Using the asymptotic analysis, we can easily conclude about the average case, best case and worst case scenario of an algorithm.

It is used to mathematically calculate the running time of any operation inside an algorithm.

Example: Running time of one operation is x(n) and for another operation it is calculated as f(n2). It refers to running time will increase linearly with increase in 'n' for first operation and running time will increase exponentially for second operation. Similarly the running time of both operations will be same if n is significantly small.

Usually the time required by an algorithm comes under three types:

Worst case: It defines the input for which the algorithm takes the huge time.

Average case: It takes average time for the program execution.

Best case: It defines the input for which the algorithm takes the lowest time.

# Asymptotic Notations:

The commonly used asymptotic notations used for calculating the running time complexity of an algorithm is given below:

Big oh Notation (Ο)

Omega Notation (Ω)

Theta Notation (θ)

Big oh Notation (O):

It is the formal way to express the upper boundary of an algorithm running time. It measures the worst case of time complexity or the longest amount of time, algorithm takes to complete their operation.
For example: If f(n) and g(n) are the two functions defined for positive integers, then f(n) is O(g(n)) as f(n) is big oh of g(n) or f(n) is on the order of g(n)) if there exists constants c and no such that:
F(n)≤cg(n) for all n≥no
This implies that f(n) does not grow faster than g(n), or g(n) is an upper bound on the function f(n).

Omega Notation (Ω):

It is the formal way to represent the lower bound of an algorithm's running time. It measures the best amount of time an algorithm can possibly take to complete or the best case time complexity.
If we required that an algorithm takes at least certain amount of time without using an upper bound, we use big- Ω notation i.e. the Greek letter "omega". It is used to bound the growth of running time for large input size.
If running time is Ω (f(n)), then for the larger value of n, the running time is at least k?f(n) for constant (k).

Theta Notation (?):

It is the formal way to express both the upper bound and lower bound of an algorithm running time.
Consider the running time of an algorithm is θ (n), if at once (n) gets large enough the running time is at most k2-n and at least k1 ?n for some constants k1 and k2.

# Searching
Searching is the process of finding some particular element in the list. If the element is present in the list, then the process is called successful and the process returns the location of that element, otherwise the search is called unsuccessful.

There are two popular search methods that are widely used in order to search some item into the list. However, choice of the algorithm depends upon the arrangement of the list.

1. Linear Search
Linear search is the simplest search algorithm and often called sequential search. In this type of searching, we simply traverse the list completely and match each element of the list with the item whose location is to be found. If the match found then location of the item is returned otherwise the algorithm return NULL.

2. Binary Search
Binary search is the search technique which works efficiently on the sorted lists. Hence, in order to search an element into some list by using binary search technique, we must ensure that the list is sorted.
Binary search follows divide and conquer approach in which, the list is divided into two halves and the item is compared with the middle element of the list. If the match is found then, the location of middle element is returned otherwise, we search into either of the halves depending upon the result produced through the match.

# Stack:

Stack is an ordered list in which, insertion and deletion can be performed only at one end that is called top.

Stack is a recursive data structure having pointer to its top element.

Stacks are sometimes called as Last-In-First-Out (LIFO) lists i.e. the element which is inserted first in the stack, will be deleted last from the stack.


# Queue:

A queue can be defined as an ordered list which enables insert operations to be performed at one end called REAR and delete operations to be performed at another end called FRONT.

Queue is referred to be as First In First Out list.

For example, people waiting in line for a rail ticket form a queue.

# Linked list:

Linked List can be defined as collection of objects called nodes that are randomly stored in the memory.

A node contains two fields i.e. data stored at that particular address and the pointer which contains the address of the next node in the memory.

The last node of the list contains pointer to the null.

# Bubble sort

In Bubble sort, Each element of the array is compared with its adjacent element. The algorithm processes the list in passes. A list with n elements requires n-1 passes for sorting. Consider an array A of n elements whose elements are to be sorted by using Bubble sort. The algorithm processes like following.

In Pass 1, A[0] is compared with A[1], A[1] is compared with A[2], A[2] is compared with A[3] and so on. At the end of pass 1, the largest element of the list is placed at the highest index of the list.

In Pass 2, A[0] is compared with A[1], A[1] is compared with A[2] and so on. At the end of Pass 2 the second largest element of the list is placed at the second highest index of the list.

In pass n-1, A[0] is compared with A[1], A[1] is compared with A[2] and so on. At the end of this pass. The smallest element of the list is placed at the first index of the list.

#
