# spawn_pkg
# Basic Shapes Robot (URDF + ROS 2 Launch)

This package contains a simple **URDF model** made from basic shapes (cube, cylinder, and sphere) along with a ROS 2 launch file to visualize the robot in RViz.  
It can also be extended to spawn the robot in Gazebo.

---

## 📂 Package Structure
└── spawn_pkg
    ├── launch
    │   ├── basic_shapes_gazebo.launch.py
    │   ├── basic_shapes_rviz.launch.py
    │   └── __pycache__
    │       ├── basic_shapes_gazebo.launch.cpython-310.pyc
    │       └── basic_shapes_rviz.launch.cpython-310.pyc
    ├── package.xml
    ├── README.md
    ├── resource
    │   └── spawn_pkg
    ├── setup.cfg
    ├── setup.py
    ├── spawn_pkg
    │   └── __init__.py
    ├── test
    │   ├── test_copyright.py
    │   ├── test_flake8.py
    │   └── test_pep257.py
    ├── urdf
    │   ├── basic_shapes.urdf
    │   ├── basic_shapes.xacro
    │   ├── shapes_basic.urdf
    │   └── shapes.urdf
    └── world
        └── home.world

---

## 📦 Requirements
- ROS 2 Humble (or newer)
- `joint_state_publisher`  
- `joint_state_publisher_gui`  
- `robot_state_publisher`  
- `rviz2`  
- `xacro`

Install missing packages:
```bash
sudo apt install ros-${ROS_DISTRO}-joint-state-publisher \
                 ros-${ROS_DISTRO}-joint-state-publisher-gui \
                 ros-${ROS_DISTRO}-robot-state-publisher \
                 ros-${ROS_DISTRO}-xacro \
                 ros-${ROS_DISTRO}-rviz2


