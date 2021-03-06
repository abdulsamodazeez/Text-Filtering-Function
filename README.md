# Text Filtering Function
## Introduction
The Text Filtering Function is a function that helps in filtering a request to share an email or a note that an email has been shared already. The function was written in python programming language.

## Definition of terms and variable used
The function was defined with the word "text_filter" which accept a sentence as an arguement. Below are other variable and terms used in the code:
1. Two keywords "share" and "email were defined in order to limit our sentence filtering to sentences that have these keywords
2. An if-elif-else statement was used to break down the conditions that must be met
## How it works
The function firstly convert the inputed sentence into a lower case form in order to avoid the issue of case sensitivity, 
Secondly, it checks if the sentence contain the two defined keywords, then if the sentence does not contain these keywords: the function returns a "None" statement else it moves to the next step,
Finaly, some request words such as "can", "want", "could", "should" e.t.c were defined and must be in or start the sentence for the fuction to return a statement that "Student wants to know if can share" else it return a statment that "Student has shared"
## How to use the code
For a code to achieve it aim, it must be able to solve the intended problem. In order to be able to use the function locally, the users should firstly clone the text_filtering function script into their current working directory, then import in their code. The code snippet below shows the various ways on how the user can import the function

~~~python

import text_filter
   #OR
from Text_Filtering import text_filter

   #TO CALL FUCTION AFTER IMPORTING
text_filter()                                   #the sentence will be inputed inside the parenthesis
  #or
Text_Filtering.text_filter()

 #Testing the function
text_filter('Am I allowed to share your email')

text_filter('I am able share your email')
~~~

## Complexity of the code
The function follows the principle of linear search algorithm which is the simplest approach employed to search for an element in a data set. It examines each element until it finds a match, starting at the beginning of the data set, until the end. The search is finished and terminated once the target element is located. If it finds no match, the algorithm must terminate its execution and return an appropriate result. Therefore the Time Complexity of the text_filtering function in it worst case i.e in Big(O) notation = O(n)

## Conclusion
The function was able to solve the task of filtering an email at the shortest possible time and it also consume less reasources which makes it to be efficient and reusable.
