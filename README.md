# TM Project
This is a cosc 312 project at UTK to create a Turing Machine for a self-chosen problem

#### Team Members: 
- Colsen Murray, Porter Dosch, Adam Abdelrahman

-------------------------------------------------------------------------------------------------------------------------------------------------------

### Problem: 
- We will create a turing machine to simulate a game of slots

### Approach: 
- Implement a Pseudo Random Number Generator (PRNG) that will generate a string of numbers based on an input seed (assumed to be current system time)
- Use that string of numbers to determine 3 symbols from a preset list of symbols, adding each to the tape as we get it
- Trace through the tape, checking for wins along the way
