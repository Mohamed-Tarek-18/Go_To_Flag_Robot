# Mission Coordination Go_To_Flag_Robot
This project showcases a simulation of three autonomous robots navigating towards three flags while avoiding collisions with three square obstacles.

**Educational Context:**  
This project was developed as a part of the **Mission Coordination for Multi-Robots** course at University of Évry, Paris-Saclay. It aims to provide practical insights into multi-robot autonomous navigationand develop stratigies for obstacles avoidance. The original repository, on which I built the stratigy, has all the required ROS files to start the simulation of the robots. 
Tt can be found on https://github.com/KTBE/Mission_Coordination_project.git.

Step 1: clone the repository.  
Navigate to a new folder in a terminal and run the following lines
```bash
cd ~/catkin_ws/src && git clone https://github.com/Mohamed-Tarek-18/Go_To_Flag_Robot.git
cd ~/catkin_ws && catkin_make && source ~/catkin_ws/devel/setup.bash
```
Step 2: Make the agent.py file executable.  
For this purpose, execute this code one after the other in the same terminal.
```bash
cd /home/user/catkin_ws/src/Mission_Coordination_project/evry_project_strategy/nodes
chmod +x agent.py
cd ~
```
Step 3: Run gazebo simulation.  
1. Open gazebo software.
2. To run the simulation, open a new terminal and run the following instruction:
```bash
roslaunch evry_project_description simu_robot.launch
```

Step 4: Run the python script containing the strategy  
In a second terminal, run the python script containing your strategy by executing:
```bash
roslaunch evry_project_strategy agent.launch
```
