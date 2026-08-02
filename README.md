# Build Meshes and non-meshes
```
# option 1
cd ~/ros2_ws
colcon build --packages-select my_box_bot_description
source install/setup.bash
ros2 launch my_box_bot_description urdf_visualize_geometric.launch.py

source ~/ros2_ws/install/setup.bash
ros2 run joint_state_publisher_gui joint_state_publisher_gui

# option 2

cd ~/ros2_ws
colcon build --packages-select my_box_bot_description
source install/setup.bash
ros2 launch my_box_bot_description urdf_visualize_meshes.launch.py

# Start the Joint State Publisher GUI to publish the joint states:

source ~/ros2_ws/install/setup.bash
ros2 run joint_state_publisher_gui joint_state_publisher_gui
```
