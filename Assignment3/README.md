# MapReduce with concurrency using Semaphores

## Steps to run the project

You must be on a Linux system to run the following program. Follow the below steps to run the files

1. Clone the repository into your local system.
2. Traverse to Assignment3 folder
3. Run the following commands:

```
make
./combiner 10 8 <input.txt
```
In case this command fails to work, use the below commands to run the program:

```
gcc -pthread -o combiner combiner.c
./combiner 10 8 <input.txt
```

# Note:
* input file provided has 8 unique userIDs
* First and the second argument passed has to be greater than zero and a whole number
* Sample output file has been included to show how the output should look like