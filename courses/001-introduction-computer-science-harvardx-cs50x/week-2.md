# Week 2
October 14-, 2014

[Problem Set 2](http://cdn.cs50.net/2015/x/psets/2/pset2/pset2.html)

## Todo
- [x] Watch Lecture
- [x] Watch Lecture Continued
- [x] Read Pages 11 – 14 and 39 of http://www.howstuffworks.com/c.htm
- [ ] Watch section video
- [ ] [Getting Ready](http://cdn.cs50.net/2015/x/psets/2/pset2/pset2.html#getting_ready)
  - [x] Loops [4/4]
  - [ ] Videos [0/14]
  - [ ] Videos [0/3]
- [ ] [Getting Started](http://cdn.cs50.net/2015/x/psets/2/pset2/pset2.html#getting_started)
- [ ] [Initializing](http://cdn.cs50.net/2015/x/psets/2/pset2/pset2.html#initializing)
- [ ] [Hail, Caesar!](http://cdn.cs50.net/2015/x/psets/2/pset2/pset2.html#hail_caesar)
- [ ] [Parlez-vous français?](http://cdn.cs50.net/2015/x/psets/2/pset2/pset2.html#parlez_vous_français)
- [ ] Check that you got everything from Week 2 on edX
- [ ] [Submit Problem Set 2](http://cdn.cs50.net/2015/x/psets/2/pset2/pset2.html#how_to_submit)

---

## Notes

### Lecture

**floating point imprecision** - Similar to how we can't accurately represent 1/3rd
in decimal numbers, a computer can't accurately represent certain numbers in
binary floating point.

**strlen** - string length. needs <string.h>

**man** - manual in command line. Can tell you which libraries you need
Example "man strlen"

I did not know you could define another variable after <code>int i = 0;</code>
```
for (int i = 0, n = strlen(s); i < n; i ++ )
```

**toupper** - converts lowercase to uppercase. needs <ctype.h>

http://reference.cs50.net

**arrays**
```
int age[n];
```

### Shorts

**How does a while loop differ from a do-while loop? When is the latter particularly useful?**

A do-while loop always runs at least once

**What does undeclared identifier usually indicate if outputted by make (or, really, clang)?**



**Why is Caesar’s cipher not very secure?**
Caesar's cipher is not secure because you only have to shift 26 times to decipher the text. Also, if someone had the key you used, it would be even easier to figure it out.

**What’s a function?**
Sections of code used within a larger program to perform a particular task.

**Why bother writing functions when you can just copy and paste code as needed?**
Because it's important to not repeat yourself when you're programming. If you found out the code you copy and pasted needed to be changed later, you would have to change every instance of that code. If you just used a function, you would only have to change it once.
