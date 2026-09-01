# ECE 2112_PA1
### This repository contains the Programming Assignment 1 for ECE 2112. The goal of this programming assignment is to apply basic Python functions and operations, such as manipulating strings using indexing, slicing, and sequence unpacking.

## Objective:
### Write a Python program in a Jupyter Notebook to solve each of the following problems.
### • Use the exact function names specified in each problem.
### • Place each problem in a separate, clearly labeled section of the notebook.
### • Each function must return the required result unless printed output is explicitly requested.
### • Do not use external Python libraries.
### • Use only basic Python operations, string methods, slicing, and sequence unpacking. Loops and classes are not required.
### • Test each function using the examples provided. Additional valid inputs may be used when grading the notebook.

## A. WORD ROTATION PROBLEM (Slicing)
### Create a function that moves the first character of the string to the end while keeping the characters in the middle in their original order. Preserve the capitalization of every character.

### Function/s used:
`rotate_word()` ### ~ this function uses splicing to remove the first element, returning the remaining elements before adding back the removed element.

``` python
def rotate_word(x):
    txt = x[1::]
    return(txt + x[0])
rotate_word("python")
```

## B. USERNAME BUILDER PROBLEM
### Create a function that accepts two strings (first.name and last.name) and must:
### 1. Convert all letters to lowercase;
### 2. Remove all spaces from the first name;
### 3. Remove all spaces from the last name; and
### 4. Join the processed first and last names using one period (.).

### Function/s used:
`make_username()` ### ~ after inputting two strings, the function will then do the following:
### • Convert all letters to lowercase
### • Remove all spaces
### • Combine the two strings using one period (.).

``` python
def make_username(x,y):
    txt1 = x.lower()
    txt2 = y.lower()
    ftxt1 = txt1.replace(" ", "")
    ftxt2 = txt2.replace(" ", "")
    ftxt = ftxt1 + "." + ftxt2
    return(ftxt)
make_username("Ana Maria", "De Leon")
```

## C. BOOKEND SWAP PROBLEM (Sequence Unpacking)
### Create a function that accepts a list (containing at least 2 elements). This function will then switch the first and last elements while keeping the order of the middle element/s intact.

### Function/s used:
`swap_bookends` ### ~ the function simply switches the first and last elements of a list.

```python
def swap_bookends(items):
    first, *middle, last = items
    return[last, *middle, first]
swap_bookends([1, 2, 3, 4, 5, 6])
```

