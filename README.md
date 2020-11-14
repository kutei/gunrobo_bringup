# gunrobo_bringup rospackage

## install dependency
```
sudo apt-get update
sudo apt install python-vcstool curl
echo "source /usr/share/vcstool-completion/vcs.bash" >> ~/.bashrc
```

## how to setup
```
mkdir -p ~/gunrobo_ws
cd ~/gunrobo_ws
curl -O https://raw.githubusercontent.com/kutei/gunrobo_bringup/master/.rosinstall
vcstool import < .rosinstall
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
