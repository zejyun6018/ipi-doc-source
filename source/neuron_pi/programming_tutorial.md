# How to ROS2 

## Installation
Install ROS2 (dashing) on ubuntu (18.04) by following the complete official [tutorial](https://index.ros.org/doc/ros2/Installation/Dashing/).

---

## Create a workspace
A workspace is able to contain an arbitrary number of packages. Normally, every project should have its own workspace. [more info](https://index.ros.org/doc/ros2/Tutorials/Colcon-Tutorial/)
### Quick hands-on
```
# Source ROS2
source /opt/ros/dashing/setup.bash

# Create a workspace directory
mkdir -p ~/ros2_ws/src

# Build the workspace
cd ~/ros2_ws
colcon build --symlink-install

# Source the workspace setup files
source ~/ros2_ws/install/local_setup.bash
```

---

## Create a package
A package can be considered a container for your ROS2 codes, including launch files, c++/python files, maps, parameter files, configs, etc. A package contains all the needed files to execute a function. [more info](https://index.ros.org/doc/ros2/Tutorials/Creating-A-ROS2-Package/#createpkg).
### Essential components
```
package/
    src/
    CMakeLists.txt
    package.xml
```
* [Introduction of CmakeLists.txt](https://index.ros.org/doc/ros2/Tutorials/Ament-CMake-Documentation/)
* [Introduction of package.xml](https://index.ros.org/doc/ros2/Tutorials/Creating-A-ROS2-Package/#customize-package-xml)


### Quick hands-on
```
# Source ROS2
source /opt/ros/dashing/setup.bash && 

# Create a ROS2 package "ros2 pkg create <package_name> --dependencies <dependencies>"
cd ~/ros2_ws/src/
ros2 pkg create cpp_pubsub --dependencies rclcpp std_msgs

# Build the package
cd ~/ros2_ws/
colcon build --symlink-install
source ~/ros2_ws/install/local_setup.bash
```

---

## Create a node 
A node is a basic unit of a ROS system. Nodes are executable processes that communicate over the ROS system. [more info](https://index.ros.org/doc/ros2/Tutorials/Understanding-ROS2-Nodes/#ros2nodes)

### Quick hands-on
* [Create c++ publisher and subscriber](https://index.ros.org/doc/ros2/Tutorials/Writing-A-Simple-Cpp-Publisher-And-Subscriber/#cpppubsub)
* [Create python publisher and subscriber](https://index.ros.org/doc/ros2/Tutorials/Writing-A-Simple-Py-Publisher-And-Subscriber/#pypubsub)

---

## Create a launch file
A Launch file allows you to start up and configure a number of executables containing ROS 2 nodes simultaneously. [more info](https://index.ros.org/doc/ros2/Tutorials/Launch-system/)
### [Quick hands-on](https://index.ros.org/doc/ros2/Tutorials/Launch-Files/Creating-Launch-Files/)

---

## ROS2 tools
### Dependency tool
* [rosdep](http://wiki.ros.org/rosdep)

### Introspection tools
ROS2 provides serveral tools for system introspection. Users are able to use them to debug, print messages, etc.
* [ros2 topic](https://index.ros.org/doc/ros2/Tutorials/Topics/Understanding-ROS2-Topics/)
* [ros2 bag](https://github.com/ros2/rosbag2)
* [ros2 node](https://index.ros.org/doc/ros2/Tutorials/Understanding-ROS2-Nodes/)
* [more info](https://index.ros.org/doc/ros2/Tutorials/Introspection-with-command-line-tools/)
