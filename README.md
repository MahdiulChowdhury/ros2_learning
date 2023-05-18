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

# how to debug ROS2 service
<mark >ros2 service list </mark> \
<mark >ros2 info /<..service topic..> </mark> \
<mark >ros2 service type <..srv folder name..> </mark> \
<mark >ros2 service show <..srv folder name/srv/service type..> </mark> 

using RQT: GUI interface visualize service topic, type 

# how to remap a service name at Runtime
add argument: --ros-args -r <..current_name..>:=new_name


# build individual package: 
<mark > colcon build --packages-select <package name></mark> 

# ros2 custom message
cd ros2_ws/install/<custom message>