# Midterm Exam for CSCI 5802 - Spring 2017 (100 points) - 15% of your grade.

## General Notes
* You need to work on this exam individually.
* The exam is due on Friday by 11:59 pm.
* Commit your solutions to the repository labeled with naming convention Solution1.md, Solution2.md etc... Any additional files used should be referenced from the corresponding Solution markdown files.
* Look through your answers a second time after you write them. Do this after you take a break from writing to make sure they still make sense to you.
* Note all assumptions made.
* Estimated time to complete: 4 hours (without interruptions). Note that the time is an average and it is very likely you might need more than 4 hours to complete this but not more than the 72 hours allocated.
* If your midterm is not submitted by Friday 11:59 it will not be graded.

## Extra Credit
As specified earlier, Hack YSU challenge solvers can get upto 30 points added to this midterm score. The deadline for submitting the challenge was 3/13.   

## How to submit
Once you are done with your midterm solutions, issue a pull request to submit your midterm and request a review by me and TA.

## Problem 1 (30 points)

a) What do each of the terms mean? (8 points)
* Checkout
* Working copy
* Branch
* Update
* Commit
* Push
* Pull
* Clone

b) What are the similarities and differences between Subversion and Git?  (2 points)

c) What is the git command to update the working copy of a repository?   What is the subversion command to update the working copy of a repository? (5 points)

d) What does conflict mean in a versioning system?  What are the cases that cause a conflict?  What do you do to resolve a conflict? Simulate a conflict in this repository and explain with an example the set of steps followed to create and resolve the conflict.  A working example showing this needs to be provided. (15 points)


## Problem 2 (30 points)

a) Name two static analysis tools and two dynamic analysis tools you have used so far. For each of these tools, give a short summary of the tool in your own words and list pros and cons of each. (10 points)

b) Run [PMD](https://pmd.github.io/) on the JFreeChart codebase and compare the results with FindBugs you did as part of assignment 2.  Write up  the similarities and differences you found between the two tools. In your write up, mention specific results that were the same and different between the two tools. If you had to choose one of these which one would it be? Support your answer. (20 points)


## Problem 3 (10 points)

Write a simple Makefile based on the following files (assume you had these files).  

* bird.cc
* birdlist.cc
* bird.h
* birdlist.h
* main.cc	(Main program)

The dependencies are
* birdlist.cc includes birdlist.h
* bird.cc includes bird.h
* main includes both bird.h and birdlist.h

You may use the g++ compiler.  You will need to compile and link separately. Draw the graph to show dependencies. When specifying the command ``make docs``, it should run doxgyen from a file named Doxyfile.  Note that you do not need to actually run these but to test if your make file works you could recreate the dependency structure above (however, that is not required as part of this problem).


## Problem 4 (10 points)
We want to use gdb to test a bug that is occurring in prog1.cc

a) What command should you issue when compiling prog1.cc? (2 points)

b) What command would you issue to start gdb after you compiled the program above? (2 points)

c) Set a breakpoint on line 10 (2 points)

d) What is the command to get the program to start running? (2 points)

e) What is the difference between the commands ``next`` and ``step``? Explain with an example (2 points)

## Problem 5 (20 points)
a) Write a script using regular expressions that converts a [camelCase](https://en.wikipedia.org/wiki/Camel_case) identifier to an underscore identifier and vice versa.  The input is a single camelCase or under_score identifier.

10 Bonus points: If you find and replace all identifiers in a source file from one style to another.

Explain how your script should run.

b) What does the following regular expression do?
```[\w\s]```

c) Rewrite the regular expression in b) using a different pattern.

d) Write a regular expression that matches all even numbers in the range 0 to 99. (Do not list all the even numbers)
