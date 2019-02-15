# mapping
地图创建

## build ##
sudo apt-get update
sudo apt-get install -y python-wstool python-rosdep ninja-build

src/cartographer-1.0.0/scripts/install_proto3.sh
sudo rosdep init
rosdep update
rosdep install --from-paths src --ignore-src --rosdistro=${ROS_DISTRO} -y
catkin_make_isolated --install --use-ninja -j3
