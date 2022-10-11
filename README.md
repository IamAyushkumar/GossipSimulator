Gossip type algorithms can be used both for group communication and for aggregate computation. 
This project is to determine the convergence of Gossip algorithms and Push-Sum Algorithm through 
a simulator based on actors written in Erlang.

Inputs: Number of Nodes , Topology to be used (which can be of type line, 2D, Imperfect 3D, Full), and algorithm to be used (Gossip or Push Sum).  
Output: Convergence time

for Bonus following are the additional inputs:
Boolean - 'ShouldTestFaultTolerancy' and 'Number of nodes' to kill if fault tolerancy is to be tested.

Team members (Authors)
Name	        UFID        emailID
Akash Kumar	    80024442    akashkumar@ufl.edu
Ayush Kumar	    54666085    ayushkumar@ufl.edu

What is working ?
Following Topologies are supported:
1. Full Network
2. Line
3. 2D Grid
4. Imperfect 3D

For 2D and Imperfect 3D topologies, the number of nodes is rounded to the square of the square root of the input nodes.

What is the largest network you managed to deal with for each type of topology and algorithm?

Type of algorithm | gossip | push-sum |
---------------------------------------
full              | 79000  | 67000    |
line              | 70     | 70       | 
2D                | 600    | 700      | 
imp3D             | 2000   | 3000     | 

Test Environment
OS: Mac OS- Monterey
Processor: Apple M2
RAM: 8.0 GB
8-core CPU with 4 performance cores and 4 efficiency cores
10-core GPU
16-core Neural Engine
100GB/s memory bandwidth

Gossip
Line: 5000. It takes about 636.657 seconds to achieve convergence
2D: 5000. It takes about 430.347 seconds to achieve convergence
full: 5000. It takes about 276.347 seconds to achieve convergence
imp3D: 5000. It takes about 421.646 seconds to achieve convergence

Push-sum
Line: 600. It takes about 1103.321 seconds (~ 18 minutes) to achieve convergence
2D: 1225. It takes about 164.639 seconds to achieve convergence
full: 1000. It takes about 3.422 seconds to achieve convergence
imp3D: 1225. It takes about 4.668 seconds to achieve convergence





