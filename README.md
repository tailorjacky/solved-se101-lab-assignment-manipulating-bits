Download Link: https://assignmentchef.com/product/solved-se101-lab-assignment-manipulating-bits
<br>
The purpose of this assignment is to become more familiar with bit-level representations and manipulations. You’ll do this by solving a series of programming “puzzles.” Many of these puzzles are quite artificial, but you’ll find yourself thinking much more about bits in working your way through them.

<h2>Logistics</h2>

You should work individually in solving the problems for this assignment. Any clarifications and revisions to the assignment will be posted on the News webpage of ICS course websit (http://ipads.se.sjtu.edu.cn/courses/ics).

<h2>Obtain Lab Materials</h2>

You should use svn tools to get lab1 from server. The operation of svn tools is similiar with its on the tutorial.

The URL of svn repository is still ”svn://ipads.se.sjtu.edu.cn/ics-se19/[account]” (the example of [account] is ”ics519021910064”). You should see a directory named ”lab1” under your path. (If you have checked out your svn directory in tutorial, you just need to update) Lab1 contains 10 files:

Makefile, README, bits.c, bits.h, btest.c, btest.h, decl.c, dlc, tests.c, and datalab.pdf

The only file you will be modifying and turning in is bits.c. The file btest.c allows you to evaluate the functional correctness of your code. The file README contains additional documentation about btest.

Use the command make to generate the test code and run it with the command ./btest. The file dlc is a compiler binary that you can use to check your solutions for compliance with the coding rules. The remaining files are used to build btest.

Looking at the file bits.c you’ll notice a C structure team into which you should insert the requested identifying information about only ONE individuals comprising your programming team. Do this right away so you don’t forget. The ”team name”and the ”login ID”are all your student id (i.e. 519021910045), and the ”student name” is the PINYIN of your name (i.e. CHEN Tianyu)

The bits.c file also contains a skeleton for each of the 15 programming puzzles. Your assignment is to complete each function skeleton using only <em>straightline </em>code (i.e., no loops or conditionals) and a limited number of C arithmetic and logical operators. Specifically, you are <em>only </em>allowed to use the following eight operators:

! ˜ &amp; ˆ | + &lt;&lt; &gt;&gt;

A few of the functions further restrict this list. Also, you are not allowed to use any constants longer than 8 bits. See the comments in bits.c for detailed rules and a discussion of the desired coding style.

<h2>Evaluation</h2>

Your code will be compiled with GCC and run and tested on one of the class machines. Your score will be computed out of a maximum of 75 points based on the following distribution:

45 Correctness of code running on one of the class machines.

30 Performance of code, based on number of operators used in each function.

The 15 puzzles you must solve have been given a difficulty rating between 1 and 4, such that their weighted sum totals to 45. We will evaluate your functions using the test arguments in btest.c. You will get full credit for a puzzle if it passes all of the tests performed by btest.c, half credit if it fails one test, and no credit otherwise.

Regarding performance, our main concern at this point in the course is that you can get the right answer. However, we want to instill in you a sense of keeping things as short and simple as you can. Furthermore, some of the puzzles can be solved by brute force, but we want you to be more clever. Thus, for each function we’ve established a maximum number of operators that you are allowed to use for each function. This limit is very generous and is designed only to catch egregiously inefficient solutions. You will receive two points for each function that satisfies the operator limit.

<h2>Advice</h2>

We recommend that you should use linux and work directly on it, which could make sure that the version you turn in compiles and runs correctly on our test machines. If it doesn’t compile, we can’t grade it.

The dlc program, a modified version of an ANSI C compiler, will be used to check your programs for compliance with the coding style rules. The typical usage is

./dlc bits.c

Type ./dlc -help for a list of command line options. The README file is also helpful. Some notes on dlc:

<ul>

 <li>The dlc program runs silently unless it detects a problem.</li>

 <li>Don’t include &lt;stdio.h&gt;in your c file, as it confuses dlc and results in some non-intuitive error messages.</li>

</ul>

Check the file README for documentation on running the btest program. You’ll find it helpful to work through the functions one at a time, testing each one as you go. You can use the -f flag to instruct btest to test only a single function, e.g., ./btest -f isPositive.

Last but not least, if you are confused by the meaning of the function, you could read the corresponding code in tests.c, which is the C version code of bits.c.

<h2>handin</h2>

You only need to commit your bits.c file, but you need to commit it at least THREE times. If you violate the rule or exceed the deadline, you can’t get any point!

<ul>

 <li>The 1st time: when you finish 5 puzzles.</li>

 <li>The 2nd time: when you finish 10 puzzles.</li>

 <li>The last time: when you finish lab1.</li>

</ul>

NOTE: There is no requirement to the order of puzzles to be done.