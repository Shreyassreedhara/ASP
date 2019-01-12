# Producer Combiner with concurrency using Mutex

## Description



## Steps to run the project

You must be on a linux system to run the following commands. Follow the steps below to run the program

1. Clone the repository to your local system
2. Head to the folder consisting of combiner and input files
3. Run the following commands:

```
make
./combiner 10 8 <input.txt
```

If for some reason the above commands do not work as expected, run the program using the below commands:

```
gcc -pthread -o combiner combiner.c
./combiner 10 8 <input.txt
```

# Author information

1. Shreyas Gaadikere Sreedhara, Email - shreyas100994@gmail.com