# MultiRobotNavigationCityFlow
This is the Repository for the Open project of the course (DTEK2084) Aerial Robotics and Multi-Robot Systems 2025 at the University of Turku. Team Members Ameer Moavia, Ayana Guruge, Syed Mehdi 
# Setup
The Following needs to be installed as a basic requirement to run the project.
1. Linux 22.04 LTS jammy jellyfish
2. ROS2 Humble Hawksbill
3. Python = 3.10
4. Cityflow v0.1 from the Git
5. OpenAI gym 0.26.2
6. stablebaselines3
   and all their dependencies.
# How to run the simulation and create a model
1. Define your configfile,flow and roadnet in /cityflow_rl/cityflow_config.
2. Then run train_city_flow.py inside the /cityflow_rl directory.
3. Model wil be created
# Visualizing cityflow
1. In order to run the replay simulation of the model, go to CityflowInstallDirectory/frontend and run index.html
2. It will open in a browser. here you can input replay_roadnet.json and replay.txt from cityflow_rl/cityflow_config
3. Run to visualize.
# Running Turtlebot3 Gazebo Environment and link
1. source ros2 and gazebo properly
   source /opt/ros/humble/setup.bash
   source /usr/share/gazebo/setup.sh
2. colcon build and source the install
3. go to /turtlebot3_ws
4. run the following
   ros2 launch multi_tb3_sim multi_turtlebot3.launch.py

## Team and credits

Open project for the course Aerial Robotics and Multi Robot Systems (DTEK2084) at the University of Turku, spring 2025, by Group 06.

Team (equal contributions): Ameer Moavia, Ayana Guruge and Syed Mehdi.

* Ameer Moavia: road network and flow files, CityFlow configuration, multi TurtleBot setup in Gazebo, ROS bridge.
* Ayana Guruge: CityFlow configuration, debugging, multi TurtleBot setup in Gazebo, ROS bridge.
* Syed Mehdi: environment setup, Gym wrapper for reinforcement learning, multi TurtleBot setup in Gazebo, ROS bridge.

Status: a DQN agent (Stable Baselines3) was trained in the CityFlow environment and three TurtleBot3 robots run in Gazebo on ROS 2 Humble. The bridge between the trained model and the TurtleBots was not finished within the course, and multi robot experiments were not run.

This repository is a copy of the original at https://github.com/Sh0w0ff/MultiRobotNavigationCityFlow, with the original commit history, dates and authors kept.
