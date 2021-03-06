## Launch Carla with option
- Go to folder `cd /opt/carla-simulator` if you install via debian package
- run sh script `./CarlaUE4.sh` without an option 

| Feature  | Option Code |
| :------------- | :------------- |
|**Run by using Nvidia Card** | `./CarlaUE4.sh -prefernvidia`|
|Low graphical details | `./CarlaUE4.sh -quality-level=Low`|
|Listen specific port |  `./CarlaUE4.sh -carla-rpc-port=N` # Listen for client connections at port `N`. Streaming port is set to `N+1` by default.|
|Specify special port for sensor data streaming| `./CarlaUE4.sh -carla-streaming-port=N` # second port will be `N+1`, use N=0 for random port|

## Carla ROS Bridge Usage
| Feature  | Option Code |
| :------------- | :------------- |
|Source ROS Bridge catkin_ws|`source ~/carla-ros-bridge/catkin_ws/devel/setup.bash`|
|Launch ROS Bridge with an example| `roslaunch carla_ros_bridge carla_ros_bridge_with_example_ego_vehicle.launch`|
|Only launch ROS Bridge| `roslaunch carla_ros_bridge carla_ros_bridge.launch`|


## MAP and Navigation
- There are 8 maps, and all of them uses [OpenDRIVE 1.4](https://www.asam.net/standards/detail/opendrive/) standarts. 
