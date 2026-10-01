# tuw_bringup
ROS2 launches


## SLAM
```
ros2 launch slam_toolbox online_async_launch.py slam_params_file:=/ ..... /tuw_bringup/config/slam_toolbox/tuw_mapper_params_online_async.yaml
ros2 run nav2_map_server map_saver_cli -f config/map/cave

```


## Nav2 demo
```
ros2 launch tuw_bringup r-mochtio.launch.py
ros2 launch tuw_bringup rviz_nav2_launch.py
ros2 launch tuw_bringup localization_launch.py map:=./ws02/src/tuw_bringup/config/map/roblab/map.yaml
ros2 launch tuw_bringup nav2_launch.py
```