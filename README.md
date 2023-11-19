# FAST_LIVO_Noetic 
## Dependency
**Livox-SDK Installation**

open New terminal 
  ```
git clone https://github.com/Livox-SDK/Livox-SDK.git
cd Livox-SDK
cd build && cmake ..
make
sudo make install
cd
git clone https://github.com/Livox-SDK/livox_ros_driver.git ws_livox/src
cd ws_livox
catkin_make
gedit ~/.bashrc
```
paste ```source ~/ws_livox/devel/setup.sh``` at the end line

**Sophus**
```
cd 
git clone https://github.com/Saifali4604/Sophus
cd Sophus
mkdir build && cd build && cmake ..
make
sudo make install
```


## Install

Use the following commands to download and compile the package.

```
cd ~/catkin_ws/src
git clone https://github.com/Saifali4604/FAST_LIVO_Noetic
cd ..
catkin_make
source ~/catkin_ws/devel/setup.bash
```
**Note:** Remember to source the catkin_ws or the work space where you have cloned 

## Run the package 
---
**Datasets for Avai:** Can be downloaded from [google drive](https://drive.google.com/drive/folders/1CGYEJ9-wWjr8INyan6q1BZz_5VtGB-fP?usp=sharing)

```
roslaunch fast_lio mapping_avia.launch
rosbag play YOUR_DOWNLOADED.bag
```
or
**Datasets for Velodyne:** Can be downloaded from [google drive](https://drive.google.com/drive/folders/1blQJuAB4S80NwZmpM6oALyHWvBljPSOE?usp=sharing) 
```
roslaunch fast_lio mapping_velodyne.launch
rosbag play YOUR_DOWNLOADED.bag
```
## 6.Acknowledgments
[https://github.com/hku-mars/FAST_LIO]
