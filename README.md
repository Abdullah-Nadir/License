
# License

## Learning Goals

- Practice working with files and file pointers
- More work with strings and arrays
- Debugging with `debug50`
- Use `valgrind` to check for memory leaks


## Background

Suppose you work for a company that develops AI-enhanced license plate recognition technology. As you develop your technology, you may want to use actual license plate numbers as test data. You have a text file with some plate numbers you want to analyze, so you first try reading from that text file and printing out the license plates, to test your file-reading logic. 

## Implementation Details

If you open the plates.txt file, you’ll notice that there are actually 8 different license plate numbers. 

First check for command-line arguments, since `argv[1]` should be the text file that contains the license plates. Then create a character array of length 7, since the plate numbers are 6 chars long and we need to save space for the NUL terminator. Now create an array of char *’s (character pointers, otherwise known as strings!) to store the 8 plate numbers. Create a file pointer to the external text file, create a variable to hold the index of each array element, and begin reading the file and saving the plate numbers to the array. Finally, to test that you did this correctly, print out the values in the array.

## Usage/Example

```c
license/ $ ./license plates.txt
11ZT00
1KAD21
78ZZ01
99ZZ11
72ZZ21
98ZZ31
44ZW41
34ZZ51
```

