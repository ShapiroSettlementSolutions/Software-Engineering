# Object are stored on the heap
# Variables are a reference to the object
# Local variables are stored on the stack

Stack is used for static memory allocation and Heap for dynamic memory allocation, both stored in the computer's RAM .


In a multi-threaded situation each thread will have its own completely independent stack but they will share the heap. Stack is thread specific and Heap is application specific. The stack is important to consider in exception handling and thread executions.

#Passing variables by value is copying object
