# Week 1
October 5-7, 2014

## Todo
- [x]Pages 1 – 7, 9, and 10 of http://www.howstuffworks.com/c.htm.
- [ ] Follow along with [Hello, C](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#hello_c)
- [ ] Watch [Shorts](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#shorts)
- [ ] [Hello again, C](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#hello_again_c)
- [ ] [Itsa Mario](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#itsa_mario)
- [ ] [Time for Change](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#time_for_change)
- [ ] [Submit Problem Set 1](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#how_to_submit)

---

## Notes

### C
<code>printf("Hello, %s", s)</code> - For printing strings
- int uses %d
- float uses %f
- char uses %c
- character strings uses %s

<code>scanf("%d", &b)</code> - Reads data and stores it

### Shorts

What’s a library? <br>
A collection of related prewritten code.

What role does ```#include <cs50.h>``` play when you write it atop some program? <br>
It's a library that you can include in your code. It has prewritten code.

What role does ```-lcs50``` play when you pass it as a "command-line argument" to clang? <br>
It links the cs50 library. Header files don't include implementation code.

#### Compiling
1. Preprocessing <i>-E</i> <br>
Includes your headers in your file
2. Compilation <i>-S</i> <br>
Compiling into assembly code
3. Assembly <i>-c</i>
4. Linking

#### Function
