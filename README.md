# fibprimes

## General

Each chord consists of one Fibonacci number and 4 (sometimes 3) primes. This was an arbitrary decision and can be altered to include more or less notes if one wishes.

For each number, the note which corresponds to it is based on its scale degree in the key of C. So, 1 corresponds to C, 2 corresponds to D, 3 corresponds to E, etc. The way the notes are assigned is described below.

## Fib

The bottom note of each 5-note chord correspond to the Fibonacci sequence mod 7 (to fit it in one octave). In the source code, the Fibonacci numbers are not generated but rather are based on an array of 16 that aligns with the cycle of the Fibonacci sequence residue class 7. In other words, the Fibonacci numbers mod 7 are cyclic after 16 numbers and that cycle is used for the bottom notes.

## Primes
The top 4 (sometimes 3) notes in the chord are generated by taking the modulo 7 of the prime numbers and assigning them to numbers (as described in General Note Assignment). However, to keep the integrity of the sequence of primes, it was necessary to spread the notes across multiple octaves (done with a simple algorithm).


## Sidenote
I am largely an elementary developer and quickly wrote this without much thought to the best programming practices. Any tips for improvement are greatly appreciated!
