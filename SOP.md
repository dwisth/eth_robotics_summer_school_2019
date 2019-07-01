## Procedure

SSH into the SMB

```bash
roslaunch new_awesome_launch_file.launch 
```

In another terminal 

```bash
rosrun apriltag_subscriber apriltag_subscriber.py
```

In yet another terminal

```bash
roslaunch ethzasl_icp_mapper supermegabot_dynamic_mapper.launch
```

The above shall run the state estimation with the Lidar
