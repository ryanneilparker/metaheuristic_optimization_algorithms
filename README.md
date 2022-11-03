# metaheuristic_optimization_algorithms
A collection of nature-inspired metaheuristic optimization algorithms 🐜

This repository contains an assortment of optimization algorithms inspired by the wonders of the natural world. 🌏

Enjoy!

## INDEX
1. [Ant Colony Optimization (ACO)](#ant_colony_optimization)
2. [Flower Pollination Agorithm (FPA)](#flower_pollination_algorithm)
3. [Particle Swarm Optimization (PSO)](#particle_swarm_optimization)
4. [Firefly Algorithm (FA)](#firefly_algorithm)
5. [Bat Algorithm (BA)](#bat_alogithm)
6. [Bee Colony Optimization (BCO)](#bee_colony_optimization)

## ant_colony_optimization
coming soon...

## flower_pollination_algorithm
coming soon...

## particle_swarm_optimization
Another popular swarm intelligence-based algorithm is PSO, which was developed by Kennedy and Eberhart in 1995 (Kennedy and Eberhart, 1995). The PSO system uses a set of multiple agents (or $n$ particles) to simulate the swarming behavior of fish and birds such as starlings. If we interpret a solution vector $x}_i$ as the position of a particle (say, particle $i$), we can also associate the motion of this particle with a velocity $ v_i$. Thus, for each particle, its position and velocity at any iteration or pseudotime $t$ can be updated iteratively using:

$$\begin{equation}  v_i^{t+1}=v_i^t+\alpha  \epsilon_1[ g^*- x_i^t]+\beta  \epsilon_2[ x_i^* -  x_i^t],\end{equation}$$
$$\begin{equation} x_i^{t+1}= x_i^t+ v_i^{t+1}\triangle t,\end{equation}$$

Where $ \epsilon_1$ and $ \epsilon_2$ are two uniformly distributed random numbers in $[0,1]$ and $t = 1$ is the time increment. Since all iterative systems can be considered as time-discrete with unit time increments, we can set $t = 1$. In addition, $ g^*$ is the best solution of the population at iteration $t$, while $ x_i^*$ is the individual best solution for particle $i$ among its search history up to iteration $t$. In addition, the learning parameters $α$ and $β$ usually take values in the range of $[0,2]$. The importance of these parameter values was analyzed and they can affect the stability of the algorithm (Clerc and Kennedy, 2002). So, it is no surprise that there are many variants (Kennedy et al., 2001).

## firefly_algorithm
FA was developed by Xin-She Yang in 2008. It is based on the swarming and light flashing behavior of tropical fireflies (Yang, 2008, 2009). In FA, a solution vector to an optimization problem is represented as the position of a firefly. The position vector $ x}_i$ of firefly $i$ at iteration $t$ is updated by:

$$\begin{equation}  x_i^{t+1}= x_i^t+\beta_0 e^{-\gamma r^2_{ij}}( x_j^t- x_i^t)+\alpha  \epsilon_i^t\end{equation}$$

where $β_0 > 0$ is the attractiveness at zero distance, that is, $r_{ij} = 0$. Though there is no best solution explicitly expressed in the equation, the fittest solution is selected from the population of $n$ solutions at each iteration. In addition, $γ$ is a scale-dependent parameter that controls the visibility of fireflies, while α controls the strength of the randomization term. The strong nonlinearity in FA can usually result in subdivision of the whole swarm into multiple subgroups or subswarms. Thus, FA is naturally suitable for multimodal optimization problems, and studies have confirmed this (Yang, 2013; Fister et al., 2013; Marichelvam et al., 2014; Osaba et al., 2017; Rango et al., 2018).

## bat_algorithm
comin soon...

## bee_colony_optimization
coming soon...
