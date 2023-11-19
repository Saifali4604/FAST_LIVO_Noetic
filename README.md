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
**Run on private dataset** Can be downloaded from ([FAST-LIVO-Datasets](https://connecthkuhk-my.sharepoint.com/:f:/g/personal/zhengcr_connect_hku_hk/Esiqlmaql0dPreuOhiHlXl4Bqu5RRRIViK1EyuR4h1_n4w?e=fZdVn0))

```
roslaunch fast_livo mapping_avia.launch
rosbag play YOUR_DOWNLOADED.bag
```
or
**Run on benchmark dataset (NTU-VIRAL)**
```
roslaunch fast_livo mapping_avia_ntu.launch
rosbag play YOUR_DOWNLOADED.bag
```
## 6.Acknowledgments
[https://github.com/hku-mars/FAST-LIVO]
