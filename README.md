**Q1**
**189636-KAYLA MAKENA MUNGA**

**Big O Notation in Algorithm Analysis**

Introduction

Big O notation is a mathematical notation that describes the upper bound of an algorithm's time complexity. It also helps in the comparison of algorithms.
Rules of Big O Notation

i. Constant Time Complexity[O(1)]
an algorithm has the constant time complexity if it's execution time usually doesn't depend on the size of input.
Example:
public static int getFirstElement(int[] arr) {
    return arr[0];
}


ii.Linear Time Complexiity [O(n)] 
An algorithm has time linear complexity if the execution time increases linearrly with the size of the input.
Example:
public static void printAll(int[] arr) {
    for (int i : arr) {
        System.out.println(i);
    }
}




iii. Quadratic Time Complexity [O(n^2)] 
A quadratic time complexity occurs when the algorithm contains nested loops that are iterating over the same dataset 
example:
public static void printAllPairs(int[] arr) {
    for (int i : arr) {
        for (int j : arr) {
            System.out.println(i + ", " + j);
        }
    }
}


iv. Logarithmic Time Complexity [O(logn)]
Alogarithmic time complexity occurs when the algorithm reduces the problem size in each step.
Example:
public static int binarySearch(int[] arr, int target) {
    int low = 0, high = arr.length - 1;

    while (low <= high) {
        int mid = (low + high) / 2;
        if (arr[mid] == target) return mid;
        else if (arr[mid] < target) low = mid + 1;
        else high = mid - 1;
    }
    return -1;
}



**Q2**
**189636-KAYLA MAKENA MUNGA** 
**Difference between arrays and linked lists**


Memory Allocation -
Arrays: all elements in arrays are usually stored next to each other in memory. they require more memory due to fixed allocation.
the size of arrays is fixed at the time of declaration therefore it is neccessary for the number to be defined beforehand.
Linked lists: all nodes in linked lists are ususally stored where one node points to the next.
nodes are created only when they are needed .


Performance-
arrays:access to arrays is in the constant time complexity because any element is directly accessible using an index. Insertions and deletions require a linear time complexity because of element shifting.
Linked lists:access to inked lists is in linear time complexity because of their linear transversal and in insertion and deletion they use constant time complexity because they reassign pointer refences without shifting any other nodes.


Insertion and deletion-
arrays: Insertion and deletion are in linear time complexity when they are performed at the beggining or middle of the array due to element shifting.
Linked Lists: insertion and deletion is in constant time complexity which is at the head or tail but have a linear time complexity while doing modifications in the middle 
