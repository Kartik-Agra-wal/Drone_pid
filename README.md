# Drone_pid
Pid control of hector drone
Time taken : 3 days
* Clone the repository in your workspace along with this repo
```
git clone https://github.com/RAFALAMAO/hector_quadrotor_noetic
```

## Package
This package contains two launch files

**1.test.launch**
This launches the hector drone in an empty world.

**2. bring_hector_drone.launch**
This launches the drone in a city world environment.

There are three scripts for the control of the drone.

_1.fly_drone.py_

This script alows the drone to hover at a certain height(1.5) based on the data from sonar sensors.

_2.test.py_

This script alows the drone to follow a list of waypoints and land on the last waypoint using PID.


https://user-images.githubusercontent.com/87862080/209577210-8553fd29-e7ed-4020-a837-aaf6538eefe7.mp4



``` 
waypoint_x = np.array([10.0, 10.0, -10.0,10.0, 0.0])
waypoint_y = np.array([0.0 , 10.0, 10.0,-10.0, 0.0])
``` 
the above list in the code can be modified to change the waypoints.Use this for the the empty world for better visualization.


_3. pid_control.py_
This script is similar to the test.py file ,it is just setup for moving from point A to B on the city environment.
```
    waypoint_x = np.array([250.0])
    waypoint_y = np.array([100.0])
```
You can change the destination points here 


https://user-images.githubusercontent.com/87862080/209577217-cf5d4eab-4fa4-4a0c-ab26-018abf7531cb.mp4


