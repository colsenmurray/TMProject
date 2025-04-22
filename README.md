# TM Project
This is a cosc 312 project at UTK to create a Turing Machine for a self-chosen problem.

The turing machine is described by a text file in this repository. These text files are only recognizable by the STEM software from Dr. Barry at the University of Tennessee.

#### Team Members: 
- Colsen Murray, Porter Dosch, Adam Abdelrahman

-------------------------------------------------------------------------------------------------------------------------------------------------------

### Problem: 
- We will create a turing machine to simulate a game of slots

### Approach: 
- Implement a Pseudo Random Number Generator (PRNG) that will generate a string of numbers based on an input seed (assumed to be current system time)
- Use that string of numbers to determine 3 symbols from a preset list of symbols, adding each to the tape as we get it
- Trace through the tape, checking for wins along the way

### Input:
- Takes an input of seeds on the tape
- The seeds can each be as many bits as desired
- Must be in binary notation
- The recognized symbols are {#, $, 0, 1}
- Input format should be of the form
    - #seed1#seed2#seed3#$

### Output:
- There are 3 possible outputs
    - Loss
    - 3 Pt Win
    - 5 Pt Win
- For each, the output is a $ followed by the corresponding points in binary
    - 0: $000
    - 3: $011
    - 5: $101
