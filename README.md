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
    


In this problem, the task to be accomplished is to move the first character of the string to the end while keeping all remaining characters in their original order. This was done by slicing the second character of the string using` "text[1:]"` from the first character , and simply appending the first character `"text[0]"` at the end by using `"+"` in order to join the two creating an output like `"ythonp"`. The slicing operator `":"` was used to gather all the remaining characters within the text or string in their original order. 




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


In this problem, a function named make_username() that accepts two strings: first name and last name, and must adhere to the conditions stated. The characters of the first and last name strings were turned into lowercase by using `".lower()"`. The `.replace(" ", "")` was used to find every space in a character `(" ")`, and replaces it with no spaces `("")`. The `return f"{clean_first}.{clean_last}"` uses an f-string to place the cleaned strings around a period. With all of these it produces an output such as `("Ana Maria", "De Leon")` to `("anamaria.deleon")`.




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

In this problem, a function named swap_bookends() that accepts a list containing at least two elements has to unpack the list into three variables: The `"first"` for the first element, the `"middle"` for the list containing everything between the first and last elements, and `"last"` for the last element. A new list must return with the first and last elements switch placement. Using the extended sequence unpacking `"first, *middle, last = items"` the `"first"` gets the first element, the `"*middle"` gathers all the items between the first and last, and the `"last"` gets the last element. Returning a new list, the first and last elements must be isolated in `"[]"` in order for them to be swapped with their values intact. The `"return [last] + middle + [first]"` combines the elements together in a new list wherein the first and last elements are switched and leaving the middle variable untouched. This results in an output such as `"[1,2,3,4,5,6]" to "[6,2,3,4,5,1]"`.



README FILE VERSION HISTORY:
August 25, 2026 Inputted initial draft for the README file
August 26, 2026 Finished Draft 
August 26, 2026 Minor adjustments 









