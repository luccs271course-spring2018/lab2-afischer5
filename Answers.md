# COMP 271 F17 002 Lab 2


# Questions

- What is the complexity of each of the four search methods in terms of array or list size n?
- What happens in the case of binary search if the array is not sorted?
- What is the purpose of constructor argument validity checking?
- What is the purpose of using the keyword `final` with variables and arguments?
- What are alternatives to using `Optional` and how do they compare?


# Answers
## 1)
- the two linear searchs are linear regardless of using lists and arrays. Thus the number of tasks to execute is some constant multiplied by n.
- the the linear funding search is the same way however it has a different constant factor.
- the binary search is logarithmic in n. meaning that the number of tasks to complete is log base 2 of n. 

## 2)
if the array is not sorted the binary search will not function correctly as the method will not always select the correct block of elements to remove from the search

## 3)
Validity checking assures that no object that would break the search, or a parameter that doesnt make sense is created. 
Meaning that a team with negative funding would make no sense and is therefore forbidden.

## 4) 
final correctness makes sure that the programmer or user does not modify arguments of a method which is in almost every case detrimental to the method. 
It is a safety feature/ reminder.

## 5)
The alternative to using final is to have a set value of an int or string be used as a null value. 
Ie. Using -1 as no value when you know all actual values are positive.
The primary difference is confusion and checking for the specific value. 
For optionals, an empty value is recognized as no value by the program, while for using things like -1 only the programmer themselves know that -1 is a no value which can casue confusion.
