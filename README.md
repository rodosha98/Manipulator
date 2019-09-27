# Manipulator - ROS Project 
It's a model of Industrial Manipulator KUKA. Full description you can read in File "Robot Description"

How to run project:
1. Open Linux console
2. Create workspace folder (Example: mkdir -p robot_ws/src)
3. Go to workspace folder (cd robot_ws)
4. Use command catkin_make 
5. Open src and put there manipulator folder
6. return to robot_ws/ and launch catkin_make again
7. Write command source devel/setup.bash
8. Use command roslaunch robot_gazebo rviz.launch to run RVIZ and command roslaunch robot_gazebo begin.launch torum model in GAZEBO
9. Enjoy
