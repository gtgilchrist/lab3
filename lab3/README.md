# Hash Hash Hash

Making thread-safe versions of a function to add elements into a hash table with multiple collisions.

## Building

Use the "make" command to build the program.

## Running

Show an example run of your (completed) program on using the `-t` and `-s` flags
of a run where the base hash table completes in between 1-2 seconds.

An example run is as follows:
./hash-table-tester -t 4 -s 120000
Which has the following output:
Generation: 78,774 usec
Hash table base: 1,715,905 usec
    - 0 missing
Hash table v1: 2,647,534 usec
    - 0 missing
Hash table v2: 509,849 usec
    - 0 missing

## First Implementation

Describe your first implementation strategy here (the one with a single mutex).
Argue why your strategy is correct.

### Performance

Run the tester such that the base hash table completes in 1-2 seconds.
Report the relative speedup (or slow down) with a low number of threads and a
high number of threads. Note that the amount of work (`-t` times `-s`) should
remain constant. Explain any differences between the two.

## Second Implementation

Describe your second implementation strategy here (the one with a multiple
mutexes). Argue why your strategy is correct.

### Performance

Run the tester such that the base hash table completes in 1-2 seconds.
Report the relative speedup with number of threads equal to the number of
physical cores on your machine (at least 4). Note again that the amount of work
(`-t` times `-s`) should remain constant. Report the speedup relative to the
base hash table implementation. Explain the difference between this
implementation and your first, which respect why you get a performance increase.

## Cleaning up

The "make clean" command deletes all the binary files.
