# ros2_learning (Udemy course: https://www.udemy.com/course/ros2-for-beginners/)
## how create workspace and package: 
1. mkdir -p my_ros2_ws/src
2. colcon build
3. source ~/my_ros2_ws/install/local_setup.bash \

C Package:\
ros2 pkg create --build-type ament_cmake <package_name> \
or 
2. ros2 pkg create --build-type ament_cmake --node-name my_node my_package

python package: 
ros2 pkg create --build-type ament_python <package_name>
or 
ros2 pkg create --build-type ament_python --node-name my_node my_package