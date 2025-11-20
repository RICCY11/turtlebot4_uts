# turtlebot4_pick_place
Source code untuk UTS RE702
Task dari project ini adalah bergerak ke titik A, mengaktifkan bel sekali (mendapatkan barang/benda kerja), lalu berpindah ke titik B dan mengaktifkan bel dua kali (barang/bendar kerja sampai tujuan).

---
# How To Build
### Create Folder Workspace
```
mkdir -p turtlebot4_ws/src
cd turtlebot4_ws/src
```
### Clone this repo 
```
git clone https://github.com/MasdikaAliman/turtlebot4_nav_point_to_point.git
```
### Install package and dependiencies
```
cd ../ && rosdep install --from-paths src --ignore-src -r -y
```
### Build the package
```
colcon build
```
---
