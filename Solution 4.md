##solution 4##
a. 
> g++ -Wall prog1.cc

b.
> % gdb broken

c. 

> (gbd) b 10

d. 

> (gdb) run

e. Step "steps" into a function whereas next will step over a function. 
Step works like next unless it is given line number information. It will continue running your program until it reaches the source line. It will stop and then return the control to GDB.

