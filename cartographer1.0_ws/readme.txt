catkin_make_isolated --install --use-ninja -j3

source install_isolated/setup.bash
 
roslaunch cartographer_ros demo_hokuyo_xx.launch 
 
rosrun map_server map_saver -f map/mymap


