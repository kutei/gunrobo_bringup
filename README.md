# gunrobo_bringup rospackage

## install dependency
```
sudo apt-get update
sudo apt install python-vcstool curl
echo "source /usr/share/vcstool-completion/vcs.bash" >> ~/.bashrc
```

## how to setup
```
mkdir -p ~/gunrobo_ws/src
cd ~/gunrobo_ws/src
git clone https://github.com/kutei/gunrobo_bringup.git
vcs import < gunrobo_bringup/.rosinstall
```

## how to build
```
cd ~/gunrobo_ws
catkin init
catkin build
```

## how to bring up only gazebo simulation
```
roslaunch gunrobo_bringup gazebo_sim.launch
```
