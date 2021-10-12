# ecse373_f21_group6_navvis_rosbags Instructions
###### ECSE 373 Lab 4 for group 6
### Dependence

This package depends on `maps_glennan` package and the `lab_4_dependence` branch of `navvis_description` package. 

Use the following command to colne `maps_glennan`:

```
git clone git@github.com:cwru-eecs-373/maps_glennan.git
```

Use the following command to colne the `lab_4_dependence` branch of `navvis_description`:

```
git clone -b lab_4_dependence git@github.com:cwru-courses/ecse373_f21_yxz2309_navvis_description.git
```
### Launch

 Parameter `use_sim_time` controls the rosmaster parameter `use_sim_time`, it defaults to `true`.
 
 Parameter `config_file` is the name of rivz configuration file it defaults to `config.rviz`.
 
 ##### Display the robot
 Use the following command to display the robot:
 ```
 roslaunch navvis_rosbags launch_file.launch use_sim_time:=false
 ```

 ##### Display the robot with laser
 Use the following command to display the robot and laser:
 ```
 roslaunch navvis_rosbags launch_file.launch config_file:=config_with_laser.rviz
 ```
 Load the bag file through rqt_bag gui, than right click the blank and select Pulish -> Publish All. Than click the play button. 
 
 ##### Display the robot with laser and map
 Use the following command to display the robot with laser and map
 ```
 roslaunch navvis_rosbags launch_file.launch config_file:=config_with_laser_and_map.rviz
 ```
 Load the bag file through rqt_bag gui, than right click the blank and select Pulish -> Publish All. Than click the play button. 
 
 In order to display the 3D map, change the `Fixed Frame` parameter in rviz from `base` to `map`. 
  
