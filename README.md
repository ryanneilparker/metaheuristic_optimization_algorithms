# metaheuristic_optimization_algorithms
A collection of nature-inspired metaheuristic optimization algorithms 🐜

This repository contains an assortment of optimization algorithms inspired by the wonders of the natural world. 🌏

Enjoy!

## INDEX
[Ant Colony Optimization (ACO)](#ant_colony_optimization)
[Flower Pollination Agorithm (FPA)](#flower_pollination_algorithm)
[Particle Swarm Optimization (PSO)](#particle_swarm_optimization)
[Firefly Algorithm (FA)](#firefly_algorithm)

## ant_colony_optimization
coming soon...

## flower_pollination_algorithm
coming soon...

## particle_swarm_optimization
Another popular swarm intelligence-based algorithm is PSO, which was developed by Kennedy and Eberhart in 1995 (Kennedy and Eberhart, 1995). The PSO system uses a set of multiple agents (or $n$ particles) to simulate the swarming behavior of fish and birds such as starlings. If we interpret a solution vector $\boldsymbol{x}_i$ as the position of a particle (say, particle $i$), we can also associate the motion of this particle with a velocity $\boldsymbol{v}_i$. Thus, for each particle, its position and velocity at any iteration or pseudotime $t$ can be updated iteratively using:

$$\begin{equation} \boldsymbol{v}_i^{t+1}=v_i^t+\alpha \boldsymbol{\epsilon}_1[\boldsymbol{g}^*-\boldsymbol{x}_i^t]+\beta \boldsymbol{\epsilon}_2[\boldsymbol{x}_i^* - \boldsymbol{x}_i^t],\end{equation}$$
$$\begin{equation}\boldsymbol{x}_i^{t+1}=\boldsymbol{x}_i^t+\boldsymbol{v}_i^{t+1}\triangle t,\end{equation}$$

Where $\boldsymbol{\epsilon}_1$ and $\boldsymbol{\epsilon}_2$ are two uniformly distributed random numbers in $[0,1]$ and $t = 1$ is the time increment. Since all iterative systems can be considered as time-discrete with unit time increments, we can set $t = 1$. In addition, $\boldsymbol{g}^*$ is the best solution of the population at iteration $t$, while $\boldsymbol{x}_i^*$ is the individual best solution for particle $i$ among its search history up to iteration $t$. In addition, the learning parameters $α$ and $β$ usually take values in the range of $[0,2]$. The importance of these parameter values was analyzed and they can affect the stability of the algorithm (Clerc and Kennedy, 2002). So, it is no surprise that there are many variants (Kennedy et al., 2001).

## firefly_algorithm
FA was developed by Xin-She Yang in 2008. It is based on the swarming and light flashing behavior of tropical fireflies (Yang, 2008, 2009). In FA, a solution vector to an optimization problem is represented as the position of a firefly. The position vector $\boldsymbol{x}_i$ of firefly $i$ at iteration $t$ is updated by:

$$\begin{equation} \boldsymbol{x}_i^{t+1}=\boldsymbol{x}_i^t+\beta_0 e^{-\gamma r^2_{ij}}(\boldsymbol{x}_j^t-\boldsymbol{x}_i^t)+\alpha \boldsymbol{\epsilon}_i^t\end{equation}$$

where $β_0 > 0$ is the attractiveness at zero distance, that is, $r_{ij} = 0$. Though there is no best solution explicitly expressed in the equation, the fittest solution is selected from the population of $n$ solutions at each iteration. In addition, $γ$ is a scale-dependent parameter that controls the visibility of fireflies, while α controls the strength of the randomization term. The strong nonlinearity in FA can usually result in subdivision of the whole swarm into multiple subgroups or subswarms. Thus, FA is naturally suitable for multimodal optimization problems, and studies have confirmed this (Yang, 2013; Fister et al., 2013; Marichelvam et al., 2014; Osaba et al., 2017; Rango et al., 2018).

## bat_algorithm
comin soon...

## bee_colony_optimization
coming soon...
