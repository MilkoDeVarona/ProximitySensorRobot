# Proximity Sensor Robot

Artificial Intelligence / Reinforcement Learning

A: DISASTER ENVIRONMENT
A category 9 earthquake has devastated city X. Buildings have been destroyed, fires erupted, structures are in danger of collapsing. Search robots have been sent into the buildings to help the search for survivors. 
The various cylindrical and cubical objects represent the destroyed furniture, rubble, and debris resulting from the earthquake. The four long cuboids that make the perimeter are the walls of a person’s apartment. The small green cuboid is a human.
 
B: IMPROVED DISASTER RECOVERY
Due to the fire, debris and falling objects caused by the earthquake it would be too dangerous and risky for humans to go inside, therefore a search robot is sent in to find survivors. This robot has two types of sensors. One sensor can recognize walls, rubble, and obstacles to avoid collisions, while the other sensor detects humans. The robot will send information to the search team about the extent of the damage done to the apartment and once it finds a human it alerts them of their presence and location. 
 
C: ARCHITECTURE
The robot’s proximity sensor is very useful in a disaster environment scenario as it can detect objects to avoid collisions, but such functionality is not enough as we must be able to detect if humans are present. To accomplish this, I added a new sensor to the front of the robot with a longer range, whose only purpose is to detect specific types of objects, which in this case are humans.
 
D: INTERNAL REPRESENTATION OF THE ENVIRONMENT
The robot is programmed to move forward in a straight line until it is in the proximity of an object, at which point it will stop its movement, backup, and adjust its course by turning slightly to the left and continue its path forward. For this scenario, the robot is also programmed to detect humans, though it can be programmed to detect any specific object we need to find. Finally, the robot also sends visual information about the interior for the search team to evaluate the best course of action.

E: REASONING, KNOWLEDGE REPRESENTATION, UNCERTAINTY, AND INTELLIGENCE
Knowledge: The robot continuously collects information from the surrounding environment through two sensors located in the front. One sensor informs the robot about objects and obstacles around it, the other sensor searches for and detects a particular type of object.
Reasoning: The robot is constantly calculating its path as the sensors feed it with information from the surrounding environment. If the sensors detect an object or obstacle within a certain distance, the robot will halt its movement, turn to change its trajectory, and move forward in a new path. This process is continuously repeated. The robot sends an alert if it detects its target.
Uncertainty: The robot has no previous knowledge of the layout it must traverse, does not know what it will find inside or in what state is the environment. The robot of is also incapable of informing about the degree of injuries sustained by the victim.
Intelligence: The robot must gather information from the surrounding environment and make appropriate real time decisions. The robot is constantly calculating and adjusting its trajectory.

F: FURTHER IMPROVEMENT
In real-life disasters the information we possess about the reality on the ground is scarce and incomplete, and it is impossible to account for all possible external factors, thus the human input on how the robot must perform its task is minimal. By using reinforcement learning (Osiński, 2022) it can learn by itself how to achieve a specific goal while performing tasks and being rewarded for the good decisions it takes. The goal is to maximize total reward. This process allows the robot to learn how to best perform its task. Adding memory and implementing a mapping feature where the robot both keeps track of the paths it has already taken and creates a map of its surroundings would be another improvement as it would minimize time wasting by not revisiting the same paths. Once this map is created the search algorithm will calculate the most optimal path for the rescue teams to take in the recovery of the subject.
