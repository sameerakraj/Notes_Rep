# Week 2 - Algorithms

__types__

| Data type | Bytes   |
| :---      |  ---:   |
| bool      | 1 byte  |
| char      | 1 byte  |
| double    | 8 bytes |
| float     | 4 bytes |
| int       | 4 bytes |
| long      | 8 bytes |
| string    | ? bytes |

_1 byte = 8 bits_

__array__

Another type of data that allows you to store multiple values of the same type back to back to back (contiguously).

    int scores[3]; // declaring an array of size 3, storing integers

      scores[0] = 72;
      scores[1] = 73;

Zero-index: to start counting at 0. Arrays in C are zero-indexed.

__strings__

A string is just an array of characters (chars).

String delimiter is the NUL (\0) character to delineate where one string ends and where the next one begins.
This sentinel value demarkates the end of the string.

0000 0000 = \0 (NUL)

__for loops__

Declare multiple variables in a _for_ loop

    for (int i = 0, n = strlen(s); i < n; i++)
    {
      ...
    }

__command line arguments__

    #include <stdio.h>

    int main(void)
    {
      ...
    }

None of our programs that we have written take command-line arguments.

Command-line arguments are words after the program name in your terminal window.

    #include <stdio.h>

    int main(int argc, string argv[])
    {
      ...
    }

argc: argument count - an integer that stores how many words, in total, the human typed at the prompt (CLI).
argv[]: argument vector - an array of all of the words the human typed at the prompt (CLI).

__exit status__

Main has an ability to signal to the user if execution was successful or not.
If you do not return a value explictly, Main automatically returns 0 if program execution was successful.
