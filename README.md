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

First, run the program as is.  Hit return (enter) to continue to the next 
output as the program runs.

Second, consider the 3-boxes problem shown here:
![3-boxes problem][readme_imgs/basic_problem.png "3-boxes problem"]

Set the Lagrange parameter to 24. Write out your new QUBO as shown.

Next, do the algebra, and write down your new QUBO.

Fourth, replace the values on lines 24-29, with the values from your new 
QUBO.

Fifth, run the program.

Sixth, 
