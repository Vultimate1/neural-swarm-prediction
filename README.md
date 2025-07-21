# neural-swarm-prediction

## What is it? 
A project aimed for detecting emergent behavior in any swarm, given the internal trajectorial data of the swarm (pose, speed), and external data (shape of the swarm at any given time).

## Steps
1. Choose a software:
  a. Python, Julia or any other GUI simulation applicable language.
  b. Need to be able to create a GUI, record data, run machine learning API, and read output of machine learning back into graph.
2. Create the swarm
  a. Created a class for individual drone agent, and for a swarm.
  b. The agent class initializes a drone instance with a positional and speed characteristics, as well as viewing characterstics.
     - This is important because a Couzin swarm simulation is founded on individual drones' perception of any adjacent swarms to be able to form a swarm based on a decentralized approach.
  c. Swarm class initializes a set of drone instances, as well as records the following characteristics of a drone swarm over time:
     - Center of mass: See Equation 1.
     - Polarization: The overall direction of the swarm based on all agents
     - Relative direction: Partitions the swarm into multiple angles, and records the agents viewed by each agent in each angular section
     - Stochastic noise: Standard deviation of the overall noise in the swarm, or the deviance from circularity, square-shape, linearity, or any given swarm shape. See all calculations for swarm in Equation 2.
4. Recording of simulation data over time
  a. 
5. 

__Equation 1. Center of mass__
  a. Record positions:
  ```p = [[agent.x, agent.y, agent.z] for agent in swarm.agent if agent.is_alive]]```
  b. Record

## Languages
 - Python:
 -   Swarm construction
 -   Simulation of swarm over time
 -   Dataset creation of swarm simulations
 -   Machine learning for emergent behavior prediction
 -   Loading of machine learning model for prediction

 - Julia
 -   NetLogo swarm creation
 -   NetLogo dataset logging and creation
