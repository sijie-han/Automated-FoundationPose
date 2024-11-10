# Automated-Foundation-Pose
Contains scripts which provide interfaces with real robots and perception pipelines. Finally will be available as a ros package wit a launch file to launch all the nodes.


# Pose estimation ROS package
Place this repo in the src folder of ros catkin ws which contains the zed camera ros wrapper
Make a conda env with the requirements
```
conda create -n foundation_pose --file fp_requirements.txt
conda activate foundation_pose
```
Then source setup.bash
```
conda activate foundation_pose
source devel/setup.bash
```
Launch the zed camra wrapper
```
roslaunch zed_wrapper zedm.launch
```
Lauch the foundation pose listener which can be triggered with skills from statemachines/simulator
```
rosrun pose_estimation pose_estimation.py
```
