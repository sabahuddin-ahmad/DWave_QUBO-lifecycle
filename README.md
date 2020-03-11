# QUBO-lifecycle
Demonstrates what happens when you send a QUBO to the D-Wave QPU

## Overview

This program takes a 3-variable QUBO function and demonstrates what goes on "behind the scenes" as it runs on the QPU.  We see:

1. The original QUBO.
2. The equivalent Ising form.
3. An embedded Ising form onto the QPU architecture using four qubits.
4. A scaled version of the embedded Ising form that is the final QMI.

At this point, the problem is run on the D-Wave QPU.  When a solution is returned, we see:

5. The QMI solution (embedded Ising solution).
6. The unembedded Ising solution, with any chain breaks resolved.
7. The equivalent unembedded QUBO solution.

Note that we use the default chain strength value in this program (value of 1).  

## Exercise

First, run the program as is.  Hit any key to continue to the next output as the program runs.

Next, try modifying the program to incorporate chain strength so that we don't see any chain breaks.  

Hint: look at the Ocean documentation to figure out an easy way to adjust the chain strength.