# TM Project
This is a project for the Finite Automata (COSC 312) class at UTK. The goal is to create a Turing Machine for a self-chosen problem. Our chosen task is to create a slot machine simulation. The machine assumes that it is given three pre-generated seeds, presumably from another program which calls this one. It then returns the score from this run.

The turing machine is described by a text file in this repository. These text files are recognizable by the STEM software from Dr. Michael Barry at the University of Tennessee.

#### Team Members: 
- Colsen Murray
- Porter Dosch
- Adam Abdelrahman

-------------------------------------------------------------------------------------------------------------------------------------------------------

### Approach: 
- Implement a Pseudo Random Number Generator (PRNG) that will generate a string of numbers based on an input seed (assumed to be current system time)
    - In the machine, this is the beige section in the bottom left
- Use a modulo function to cut these numbers down to three sets of 3 bit numbers
    - This section is the rainbow-colored section in the top left of the machine
- Trace through the tape, checking for wins (duplicate numbers) along the way
    - This secgtion is the pastel colored section on the right of the machine

### Input:
- Takes an input of seeds on the tape
- The seeds can each be as many bits as desired
- Must be in binary notation
- The recognized symbols are {`#`, `$`, `0`, `1`}
- Input format should be of the form
    - `#seed1#seed2#seed3#$`
    - ex. `#10101#01#01101#$`

### Output:
- There are 3 possible outputs
    - Loss
    - 3 Pt Win
    - 5 Pt Win
- For each, the output is a $ followed by the corresponding points in binary
    - 0: `$000`
    - 3: `$011`
    - 5: `$101`
