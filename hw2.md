### ENGR 399 - ROS Independent Study

# HW2

#### Goals: Write 2 nodes that will command the robot to traverse two paths of specific shapes. Get accustomed to the github workflow.

**1.** Create a package called `cmd_vel_publisher` with `rospy` as a dependency.

**2.** Create a Github repository called `cmd_vel_publisher`. In the github repo description, put 

> HW2 for ROS Independent Study. Writing publisher nodes that command the robot to move in specific shapes.

In the README.md, include these instructions. 

**3.** Initialize a `.git` repository in the package folder (ie. `catkin_ws/src/cmd_vel_publisher/`). Add your github repository as a remote. Add the changes, commit with the message `init`, and push the package to your github repository.

**4.** Write a node `infinity_node.py` that makes the robot drive in an infinity path. Model the path as two conjoined **perfect** circles (radius of 2m) like the track shown below. The point of conjuction (where it crosses from one circle to the next) must be the same for the clockwise and anticlockwise crossings. 

<p align="center">
<img src="https://previews.123rf.com/images/hobbitfoot/hobbitfoot1704/hobbitfoot170400553/76356653-track-road-infinity-road-vector-highway-vector-illustration-speedway-background-.jpg" width="369" height="369" title="Infinity Track">
</p>

**5.** Add, commit and push after completing `infinity_node.py`

**6.** Write a node that makes the robot drive in an uncircumscribed pentagram. Use the image below for the order in which the path is traversed. At each vertex, the robot must come to a complete stop, and rotate 36 degrees (internal angle of pentagram vertex). 

<p align="center">
<img src="http://hermeticherald.com/wp-content/uploads/2018/04/Counter-Clockwsie-Pentagram-Elemental-Symbols-Diagram-300x294.png" width="369" height="369" title="Pentagram Track">
</p>

**7.** Add, commit and push after completing `pentagram.py`

**8.** Create a separate launch file for each node: `infinity.launch` and `pentagram.launch`

**9.** Add, commit and push after completing the launch files.

**TIP:** It might be useful to print the current trajectory of the robot in the console for debugging purposes.
