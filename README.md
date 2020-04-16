# stack2
Convert a Decimal Number to a Binary Number
Write a C program that reads a decimal number, and using a stack, converts it to its binary equivalent, and prints it. 
Run the program 5 times, using 5 different (some small, some large) decimal numbers.

For example, the decimal number 23310 and its corresponding binary equivalent 11101001 are interpreted respectively as
2×102+3×101+3×100
and
1×27+1×26+1×25+0×24+1×23+0×22+0×21+1×20

To convert a decimal number to an equivalent binary number, an algorithm called “Divide by 2” can be used. The algorithm uses a stack to keep track of the digits for the binary result.
The Divide by 2 algorithm assumes that we start with a positive integer. A simple iteration then continually divides the decimal number by 2 and keeps track of the remainder. The first division by 2 gives information as to whether the value is 0 or 1. 
For example, 233/2 =116 and 233%2=1
            116/2 = 58 and 116%2=0
            58/2=29 and 58%2=0
            29/2=14 and 29%2=1
            14/2=7 and 14%2=0
            7/2=3 and 7%2=1
            3/2=1 and 3%2=1
            1/2=0 and 1%2=1
We can store the remainder sequence (1 0 0 1 0 1 1 1) in a stack.
The result of converting 233 to its binary equivalent is the reverse of what is stored in the stack, that is,
(11101001).
