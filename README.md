---
tags: cssi, lists, loops
level: 2
languages: python
---
#Python Lists and Loops

#Objectives:
+ Create a list in python syntax
+ Create a loop in python syntax

#Motivation:
When we learned Javascript, we raced through lots of techniques programmers use to represent and manipulate data. We learned arrays, conditionals, looping, functions, and objects really quickly, and we used them to do interesting things to webpages.

Most of the techniques, though, don't just apply to javascript. Just like we can use the python interpreter like the javascript console, and just like we can do basic arithmetic and string operations in both languages, we can use python logic to solve problems. We'll look at the most frequently used data structures and techniques, and use them to tackle some interesting challenges.

#Lists
A list is the most basic python data structure. It is a list of objects or values. The syntax for a list is a set of objects enclosed in brackets. To create an empty list, set a variable equal to empty brackets:
```
>>> empty_list = []
```
To create a list with some elements in it, just add the elements separated by commas:
```
>>> groceries = ['Eggs', 'Milk','Butter']
```
Accessing items in a list
List items have an index and are accessed like they were in javascript:

```
>>> groceries[0]
'Eggs'
>>> groceries[1]
'Milk'
>>> groceries[0:2]
['Eggs', 'Milk']
>>> groceries[1:]
['Milk', 'Butter']
```
#Student Practice: Lists
What would this print? Why?
```
>>> groceries[0][3]
```
#Modifying a list
The easiest way to modify a list’s content is to just access the list element by its index (numerical place in the list) and use the assignment operator.
```
>>> groceries
['Eggs', 'Milk','Butter']
>>> groceries[0] = 'Bread'
>>> groceries
['Bread', 'Milk', 'Butter']
```
Another convenient way to modify a list is the append() method. The append method allows you to stick an element at the end of a list.
```
>>> groceries.append('Asparagus')
>>> groceries
['Bread', 'Milk', 'Butter', 'Asparagus']
```

#List Methods
Using the len function, you can return the number of items in a list:
```
>>> print len(groceries)
3
```
Here are some other list methods that will come in handy:
```
groceries.append('Asparagus')
['Bread', 'Milk', 'Butter', 'Asparagus']

groceries.extend(['Rutabaga', 'Ice Cream'])
['Bread', 'Milk', 'Butter', 'Asparagus','Rutabaga', 'Ice Cream']

del groceries[3]
['Bread', 'Milk', 'Butter','Rutabaga', 'Ice Cream']

groceries.remove('Rutabaga')
['Bread','Milk','Butter','Ice Cream']

groceries.sort()
['Bread', 'Butter', 'Ice Cream', 'Milk']
```

# 'In' and 'Not' Operator
What if you have a list of groceries and you want to check if ‘apples’ is in that list? Or a list of names and you want to check to see if someone is present? Use the 'in' operator.
```
if 'albert' in students:
 print 'good, albert is here'
else:
 print 'gosh, where is albert?!'
```
To check if an element is absent from a list, use the 'not' in operator:
```
if 'albert' not in students:
 print 'where is albert?!'
```

#range(): building lists of numbers easily
It is frequently useful to be able to generate a list of numbers. Rather than have you type out all the numbers you want, Python makes this easy:
```
>>> print range(0,10)
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
>>> print range(0,100,10)
[0, 10, 20, 30, 40, 50, 60, 70, 80, 90]
```
Generally, ranges have the form:
`range(<start_int>, <end_int>, <interval>)`

#Loops
Computers, as we've been learning, aren't that clever. However, they can do simple things really really fast. It makes sense that some of the most powerful things we do with computers, we do in a loop. Loops let us repeat a section of code over and over, even if we only type it out once. In javascript, we saw how to use loops to iterate through an array. We can do the same thing in python, stepping through each element in a list and doing something with it:

The simplest looping situation is where you need to do something once for every item in a list. To do this, Python uses a for loop:

#For Loops

#While Loops

#Conclusion
