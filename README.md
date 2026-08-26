# ECE2112_PA1
Made and Submitted By Steven Andrew A. Cruz of 2ECE-D
This repository contains the code for the first programming assignment of the course ECE2112 SY 2026-2027. This assignment is Experiment #1 Introduction to Python, which tackles 3 different problems using basic python functions, operators, and string operations.



Problem A.: Word Rotation Problem 
 Create a function named rotate_word() that accepts a non-empty string. Move the first character
of the string to the end while keeping all remaining characters in their original order. Preserve the
capitalization of every character.


The Methods / Functions used: 


```python

def rotate_word(text):               
    return text[1:] + text[0]
    
```
    


In this problem, the task to be accomplished is to move the first character of the string to the end while keeping all remaining characters in their original order. This was done by slicing the second character of the string using` "text[1:]"` from the first character `"text[0]"`, and simply appending the first character at the end by using `"+"` in order to join the two together creating an output like `"ythonp"`. The slicing operator `":"` was used to gather all the remaining characters within the text or string and keep them in their original order. 




Problem B.: Username Builder Problem 
Create a function named make_username() that accepts two strings: first name and last name. The
function must:
1. convert all letters to lowercase;
2. remove all spaces from the first name;
3. remove all spaces from the last name; and
4. join the processed first and last names using one period (.).


The Methods / Functions used:

```python
def make_username(first_name, last_name):
    clean_first = first_name.lower().replace(" ", "")
    clean_last = last_name.lower().replace(" ", "")
    return f"{clean_first}.{clean_last}"

```


This problem requires a function named make_username() that accepts two strings: first name and last name, and must adhere to the conditions stated. The characters of the first and last name strings were turned into lowercase by using `".lower()"`. The `.replace(" ", "")` was used to find every space in a character `(" ")`, and replaces it with no spaces `("")`. The `return f"{clean_first}.{clean_last}"` uses an f-string to place the cleaned strings around a period. With all set in place it produces an output such as `("Ana Maria", "De Leon")` to `("anamaria.deleon")`.




Problem C.: Bookend Swap Problem 
Create a function named swap_bookends() that accepts a list containing at least two elements. Unpack
the list into three variables:

• first – the first element;

• middle – a list containing everything between the first and last elements; and

• last – the last element.

Using these variables, return a new list in which the first and last elements have exchanged positions.
The elements in middle must remain in their original order. Do not modify the input list.


The Methods / Functions used: 

```python
def swap_bookends(items):
   
   first, *middle, last = items 
    return [last] + middle + [first]
    
```

This problem focuses on reconfiguring the order of the 2 elements in a list. The list must be unpack into 3 variables, which are `first` for the first element, `last` for the last element, and `*middle` for the rest of the list in between the first and last elements. The `first, *middle, last = items` line of code is called an Extended Sequence Unpacking, which gathers all of the items from the 3 variables and put them into a new list. Since the task requires the first and last elements to be switched, The line of code `return [last] + middle + [first]` is used to isolate the 2 elements `(first and last)` by using `[]` and change their positions. The operator `(+)` is used to combine the three variables, and forms a new list. This would result in an output such as `[1,2,3,4,5,6]` to `[6,2,3,4,5,1]`.  



README FILE VERSION HISTORY:
August 25, 2026 Inputted initial draft for the README file
August 26, 2026 Finished Draft 
August 26, 2026 Minor adjustments 
August 27, Applying Highlights and Quoting Code
August 27, Finishing Final Output 








