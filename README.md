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
9. Enjoy!

________________________________________________________________________________________________________________________________

Second Part - Create a model using Xacro (manipulator_xacro folder). I used xacro in order to parameterize the sizes of the links of robots, and easily change the rotation angles of each rotational joint. I also used a macro to set the same moment of inertia for each link by default, however this is temporary

How to run project:
1. Open Linux console
2. Create workspace folder (if you want use previous workspace, delete manipulator folder) (Example: mkdir -p robot_ws/src)
3. Go to workspace folder (cd robot_ws)
4. Use command catkin_make 
5. Open src and put there manipulator folder
6. return to robot_ws/ and launch catkin_make again
7. Write command source devel/setup.bash
8. Use command roslaunch robot_gazebo rviz.launch to run RVIZ and command roslaunch robot_gazebo begin.launch torum model in GAZEBO
9. Enjoy!

If you want to makechanges in manipulator's configuration:
1. Open robot.xacro in directory ./src/manipulator_xacro/robot_description/urdf
2. Change parametres
3. Go to that directory in console (cd ./src/manipulator_xacro/robot_description/urdf)
4. Generate urdf file using command: xacro robot.xacro -> robot.urdf
5. Enjoy

