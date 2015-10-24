# Week 1
October 8-14, 2014

[Problem Set 1](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html)

## Todo
- [x] Pages 1 – 7, 9, and 10 of http://www.howstuffworks.com/c.htm.
- [x] Follow along with [Hello, C](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#hello_c)
- [ ] Watch [Shorts](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#shorts)
 - [x] Boolean Values
 - [x] Compilers
 - [x] Functions
 - [x] Libraries
 - [x] Loops
 - [x] Make, Clang
 - [x] Precedence
 - [x] Style
 - [x] Typecasting
 - [x] Variables
- [x] [Hello again, C](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#hello_again_c) [11/11]
- [x] [Itsa Mario](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#itsa_mario)
- [x] [Time for Change](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#time_for_change)
- [x] [Submit Problem Set 1](http://cdn.cs50.net/2015/x/psets/1/pset1/pset1.html#how_to_submit)

---

## Notes

### C
<code>printf("Hello, %s", s)</code> - For printing strings
- int uses %d
- float uses %f
- char uses %c
- character strings uses %s

<code>scanf("%d", &b)</code> - Reads data and stores it

#### Functions

```
int square(int x)
{
  return x * x;
}
```

Functions start with a keyword to describe which type of value it returns. If the function starts with <code>void</code>, that means it doesn't return anything.

##### main

```
int main(void)
{
  return 0;
}
int main(int argc, char* argv[])
{
  return 0;
}
```
The return type is always int and returning 0 means it ran successfully. If it returns any other value, it means there was an error.

The second example is for when arguments are passed into your program through the command line. <code>argv</code> contains the arguments passed in and <code>argc</code> is the length of argv.

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

#### Make and Clang

When you run <code>clang hello.c</code>, it compiles to <code>a.out</code> and that might not be what you want. If you add the -o flag, it will do the renaming for you.

```
clang hello.c -o hello
```

##### Warnings
Warnings in clang can be defined by using <code>-W</code> flags

- <code>-Wunused-variable</code> will show a warning if there are unused variables in your code.
- <code>-Wall</code> turns on all warnings and is enabled by default with <code>make</code>
- <code>-Werror</code> stops clang from creating an executable file

##### Linking

```
clang hello.c -lcs50 -o hello
```

Make sure to include your -l options at the end.

##### Precedence

1. ( )
2. * /
3. + -

There are 2 types of decrement and increment operators:
1. prefix form - the current value is used in the expression, and then it is incremented
2. suffix form - the current value is incremented or decremented first, and then it is used in the expression

Pointer Notation
- \* dereference operator - priority over basic math operators, but not over the suffix incement and decrement operators

```
int x = 7;
int *y = &x;
```

##### Typecasting

Typecasting is converting one datatype to another

```
float x = 3.7;
(int)x;
```

Implicit casting

The computer will cast values to different types to manipulate them

```
5 + 1.1
(float)5 + 1.1
```
