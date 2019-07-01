## Procedure

SSH into the SMB

(Note: Just incase the other teams have made any changes to the config file, it is a good idea to copy our config file)
```bash
scp smb_calibration.cfg smb@11.0.0.5:/home/smb/catkin_ws/src/eth_robotics_summer_school_2019/summer_school_private/smb_confusor/config/
scp -r apriltag_subscriber smb@11.0.0.5:/home/smb/catkin_ws/src/
```

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
