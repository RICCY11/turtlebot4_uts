# turtlebot4_pick_place
Source code untuk UTS RE702
Task dari project ini adalah bergerak ke titik A, mengaktifkan bel sekali (mendapatkan barang/benda kerja), lalu berpindah ke titik B dan mengaktifkan bel dua kali (barang/bendar kerja sampai tujuan).

---
# Langkah-langkah dalam menjalankan source code
### Buat Folder Workspace
```
mkdir -p turtlebot4_ws/src
cd turtlebot4_ws/src
```
### Clone Repo 
```
git clone https://github.com/MasdikaAliman/turtlebot4_nav_point_to_point.git
```
### Build 
```
colcon build
```
---
### Koneksikan PC ke Turtlebot4
```
ssh ubuntu@192.168.185.3 
```
### Jalankan localization launch & navigation launch (pada turtlebot4)
```
source install/setup.bash
ros2 launch turtlebot4_pick_place localization.launch.py
```
```
source install/setup.bash
ros2 launch turtlebot4_pick_place uts_nav.launch.py
```
### Jalankan Rviz (pada PC)
```
ros2 launch turtlebot4_viz view_robot.launch.py # This Humble
```
### Jalankan node program pick & place nya (pada turtlebot4)
```
source install/setup.bash
ros2 run turtlebot4_pick_place turtlebot4_pick_place_node
```


