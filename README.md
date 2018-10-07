# shuffled_frog_leaping_algorithm

Shuffled Frog Leaping Algorithm (SFLA) is a memetic meta-heuristic developed for combinatorial optimization by Eusuff and Lansey in 2003.
It is a random search algorithm inspired by natural memetics which provides high performance by integrating the potential advantages of both the Memetic Algorithm (MA) and the Particle Swarm Optimization (PSO) algorithm.
SFLA is based on the evolution of memes that are carried by individuals and exchange of information globally within a population due to interaction between the individuals.
The population in SFLA is composed of a set of frogs that are organized into diverse clusters, called the memeplexes.
Each frog in the memeplex denotes a potential solution to a given optimization problem.
Within every memeplex, each of the constituent frogs holds beliefs that are influenced by the beliefs of other frogs and cultivated through a process of memetic evolution, called the local search.
Subsequent to a number of memetic evolutionary steps, the memeplexes are shuffled which leads to a global evolution.
These processes of local search and shuffling continue till the pre-defined convergence criteria are not met.
SFLA firstly generates an initial, random population P of frogs Fi of size n.
After computing the fitness of the initial solutions, the entire population is sorted in the descending order of their fitness values.
Subsequently, the frogs (Fi) are divided into m memeplexes M1, M2, M3…Mm  as follows:
Within each memeplex, the fitness of worst solution is improved by adjusting the fitness landscape according the local and global best. At this stage, if the fitness of solution improves, it replaces the worst solution else a new solution is generated at random to replace the least fitted solution.
In the pseudo-code, Dmax is the maximum allowed change in a frog’s position and rand() is a function that generates a random number between 0 and 1.
