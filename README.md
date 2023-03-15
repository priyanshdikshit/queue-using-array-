# Queue using Array

## Introduction :
A queue in C is basically a linear data structure to store and manipulate the data elements. It follows the order of First In First Out (FIFO).
In queues, the first element entered into the array is the first element to be removed from the array.
A queue is open at both ends. One end is provided for the insertion of data and the other end for the deletion of data.
</br>
A real-world example of queue can be a single-lane one-way road, where the vehicle enters first, exits first. More real-world examples can be seen as queues at the ticket windows and bus-stops.
![image](https://user-images.githubusercontent.com/125560933/221842144-592cc671-b039-4021-828f-14c5f295f303.png)

## Operations Associated with a Queue in C:

**enqueue()**: It inserts elements to the end of the queue.</br>
**dequeue()**: Removes the element from the frontal side of the queue.</br>
**Front**: Pointer element responsible for fetching the first element from the queue</br>
**Rear**: Pointer element responsible for fetching the last element from the queue</br>

## Algorithm: 
1.	Declare and set the variable front and rear to -1 initially when queue is empty.
2.	Declare the functions : Enqueue , dequeue , Display. 
3.	Give the options to user in main function to either choose the operation enqueue , dequeue, display ,exit and call the function’s accordingly. 
4.	Define the functions:

         Enqueue:
         1.	Check if the rear ==(size_of_array- 1);
          If True : print overflow
         2.	Else 
          If front == -1 , set front = 0. </br>
          Increment the value of rear and insert the data input from user into the array[rear].</br>

        Dequeue: 
         1. Check if (front==-1) or (front> rear ), if true print underflow 
         2.	Else if ( front==rear)</br>
         Set front and rear back to -1 i.e empty queue . 
         3.	Else</br> 
         set (front=front+1 )

        Display: 
          1.	If front==-1 , print queue is empty 
          2.	Else print the array queue using a for loop with
          counter variable initially set to front incrementing value upto rear .
![image](https://user-images.githubusercontent.com/125560933/221842241-5d3e14de-cdfb-4b1f-b33e-71ffba901332.png)


## Applications of Queue Data Structure
•	CPU Scheduling</br>
•	Disk Scheduling</br>
•	Asynchronous data transfer between processors such as File IO, etc.</br>
•	Breadth-First Search Algorithm (BFS)</br>
