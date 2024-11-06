# Emergent-Cooperative-Strategies-for-Multi-Agent-Shepherding-via-Reinforcement-Learning

*Abstract: We present a decentralized reinforcement learning (RL) approach to address the multi-agent shepherding control problem, departing from the conventional assumption of cohesive target groups. %(e.g., flocking targets). 
Our two-layer control architecture consists of a low-level controller that guides each herder to contain a specific target within a goal region, while a high-level layer dynamically selects from multiple targets the one an herder should aim at corralling and containing. Cooperation emerges naturally, as herders autonomously choose distinct targets to expedite task completion. We further extend this approach to large-scale systems, where each herder applies a shared policy, trained with few agents, while managing a fixed subset of agents.*

This repository contains the numerical simulations discussed in [1], demonstrating validation examples of a learning-based approach to the shepherding control problem. In this context, a group of herder agents works to corral and contain a group of target agents within a goal region in the plane.

Folder organization:

- "n1m1_example.mp4": This video corresponds to the simulation in Section IV.B, shown in inset (a) of Figure 2 in [1]. A single herder (blue diamond) corrals and contains a single target (magenta dot) within the goal region (black circle), successfully completing the task.
  
- "n2m5_example.mp4": This video illustrates the example discussed in Section VI of [1]. Here, two herders (blue diamonds) corral and contain five targets (magenta dots) within the goal region (black circle). The herders exhibit cooperative behaviors, efficiently selecting different targets to corral and completing the task.

- "n10m100_example.mp4": This video shows the simulation discussed in Section VI.A and depicted in Figure 6 of [1]. The previously trained network, designed for a two-herder, five-target scenario, is extended to handle 10 herders and 100 targets. Each herder is limited to sensing the five closest targets and the nearest herder, demonstrating the scalability and effectiveness of the proposed solution.

[1]: Italo Napolitano, Andrea Lama, Francesco De Lellis, Mario di Bernardo, "Emergent Cooperative Strategies for Multi-Agent Shepherding via Reinforcement Learning," submitted for pubblication in the proceedings of, and presentation at the European Control Conference 2025.
