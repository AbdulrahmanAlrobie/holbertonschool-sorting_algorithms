# holbertonschool-sorting_algorithms
Sorting Algorithms
This repository contains C functions for sorting algorithms, developed as part of the Holberton School curriculum.
This project is meant to be done by groups of two students. Each group should pair program for at least the mandatory parts.

Background Context
Understanding sorting algorithms is crucial for efficient programming. In this project you will implement several sorting techniques and gain a solid understanding of:

At least four different sorting algorithms.

Big O notation and how to evaluate the time complexity of an algorithm.

How to select the best sorting algorithm for a given input.

What is a stable sorting algorithm.

Resources
Before starting the project, you should review the following:

Sorting algorithm

Big O notation

Sorting algorithms animations

15 sorting algorithms in 6 minutes (video)
(Warning: This video may trigger seizures in some individuals.)

Learning Objectives
By the end of this project, you are expected to be able to explain without the aid of Google:

How each of the implemented sorting algorithms works.

The time complexity (Big O notation) in the best, average, and worst cases.

How to choose the optimal sorting algorithm based on input size and data distribution.

The concept of stable vs. unstable sorting algorithms.

Requirements
Editors: Allowed editors are vi, vim, or emacs.

Compilation:
All files will be compiled on Ubuntu 20.04 LTS using gcc with the following options:
-Wall -Werror -Wextra -pedantic -std=gnu89

Style:
Your code must conform to the Betty style guidelines (checked with betty-style.pl and betty-doc.pl).
All your files should end with a new line.

Project Files:

Your function prototypes must be declared in a header file called sort.h (which must be include guarded).

You are not allowed to use global variables.

Each file should contain no more than 5 functions.

You are not allowed to use standard library functions like printf, puts, etc., except in the provided testing files.

You may use _putchar for your own output if needed.

Additional Notes:

A list/array does not need to be sorted if its size is less than 2.

The provided testing files (e.g., main.c, print_array.c, print_list.c) will be compiled with your sorting functions during evaluation.

Do not push your own main.c files; we will use our own.

Project Tasks
0. Bubble Sort (Mandatory)
File: 0-bubble_sort.c

Function Prototype:
void bubble_sort(int *array, size_t size);

Description:
Write a function that sorts an array of integers in ascending order using the Bubble Sort algorithm.
Note: You must print the array after each swap.

Big O:
Write a file 0-O that contains three lines, one for each notation:

Best case

Average case

Worst case

1. Insertion Sort (Mandatory)
File: 1-insertion_sort_list.c

Function Prototype:
void insertion_sort_list(listint_t **list);

Description:
Write a function that sorts a doubly linked list of integers in ascending order using the Insertion Sort algorithm. You are not allowed to modify the integer n of a node; you must swap the nodes themselves.
Note: Print the list after each swap.

Big O:
Write a file 1-O with three lines for the best, average, and worst case complexities.

2. Selection Sort (Mandatory)
File: 2-selection_sort.c

Function Prototype:
void selection_sort(int *array, size_t size);

Description:
Write a function that sorts an array of integers in ascending order using the Selection Sort algorithm.
Note: Print the array after each time you swap two elements.

Big O:
Write a file 2-O with three lines for the best, average, and worst case complexities.

3. Quick Sort (Mandatory)
File: 3-quick_sort.c

Function Prototype:
void quick_sort(int *array, size_t size);

Description:
Write a function that sorts an array of integers in ascending order using the Quick Sort algorithm. You must implement the Lomuto partition scheme, using the last element as the pivot.
Note: Print the array after each swap.

Big O:
Write a file 3-O with three lines for the best, average, and worst case complexities.

Data Structures & Provided Functions
You must declare the prototypes of the following functions in your sort.h header file:

void print_array(const int *array, size_t size);
Prints an array of integers.

void print_list(const listint_t *list);
Prints a doubly linked list of integers.

Also, use the following data structure for the doubly linked list:

c
Copy
/**
 * struct listint_s - Doubly linked list node
 *
 * @n: Integer stored in the node
 * @prev: Pointer to the previous element of the list
 * @next: Pointer to the next element of the list
 */
typedef struct listint_s
{
    const int n;
    struct listint_s *prev;
    struct listint_s *next;
} listint_t;
GitHub Repository
Repository Name: holbertonschool-sorting_algorithms

Each project repository should be unique per group. Make sure you follow the naming guidelines to avoid conflicts.

Testing
Use Random.org or similar tools to generate large sets of random integers to test your sorting algorithms.

Your project will be compiled on Ubuntu 20.04 LTS with the provided files and flags. Ensure all files end with a new line.

How to Compile (Example)
To compile and test the Bubble Sort function, you might use:

bash
Copy
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 0-main.c 0-bubble_sort.c print_array.c -o bubble
./bubble
Replace the file names as appropriate for each sorting algorithm.

Conclusion
This project will help you understand different sorting algorithms and their time complexities, as well as how to analyze them using Big O notation. Work closely with your partner to ensure that all mandatory tasks are completed correctly and in a timely manner. Good luck and happy sorting!
