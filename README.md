# qt_ros2_demo
a demo for ros2 and qt5 in ubuntu22.04 ros2 humble

进入ros2_qt_demo 文件夹，创建build文件夹
```shell
ros2_ws01/src/ros2_qt_demo$ tree
.
├── build
├── CMakeLists.txt
├── include
│   ├── mainwindow.h
│   └── rclcomm.h
├── package.xml
├── resource
├── src
│   ├── main.cpp
│   ├── mainwindow.cpp
│   └── rclcomm.cpp
└── ui
    └── mainwindow.ui

5 directories, 8 files
```
ros2_qt_demo功能包编译
```shell
cd build/
cmake ..
make
```
camera、qt_pub、qt_sub功能包编译
```shell
cd ~/dev_ws/src
colcon build
```

运行

ros2_ws01/src/ros2_qt_demo/build$
```shell
./ros2_qt_demo
```

自定义订阅者
```shell
ros2 run qt_sub qt_sub
```

自定义发布者
```shell
ros2 run qt_pub qt_pub
```

摄像头节点
```shell
ros2 run camera camera_node
```
# preview
![2023-04-21_18-38](https://user-images.githubusercontent.com/33952798/233620873-a91bf43f-4caf-431a-b08d-591d4bc732b7.png)

![2023-04-21_18-44](https://user-images.githubusercontent.com/33952798/233621037-e2d03b61-28e2-4547-8826-80d29f70fa01.png)
