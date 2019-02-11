### ENGR 399 - ROS Independent Study

# HW1  

#### These questions are based only on aspects you encountered in Unit 0, Unit 1 and Unit 2. There's nothing here that wasn't part of the exercises in those units. 

**1.** Create a package called `yourFirstName_hw1` with `rospy` as a dependency.

**2.** Create a `launch` directory in your package and create a launch file called `yourFirstName_hw1.launch`.  Copy the contents of `keyboard_teleop.launch` file from the `turtlebot_teleop`  package into the launch file. Ensure your launch file launches the same turtlebot teleop controls as seen in the lesson using `roslaunch yourFirstName_hw1 yourFirstName_hw1.launch`.

**3.** Edit your launch file such that the name of the teleop node launched is `yourFirstName_teleop_node`; and change the default *linear* and *angular* velocities to **0.69** and **1.23** respectively.

**4.** In the `src` directory of your package, create a python script called `yourFirstName_hw1.py`. Write a script that initializes a node called `Greetings` and prints **"Hello World!"** *every* **2** *seconds*.

**5.** Edit your launch file so that alongside the teleop node, your `yourFirstName.py` script is launched and creates a node named `firstName_Greetings`.

**6.** Compress your package folder into a `.zip` file called `yourFirstName_hw1.zip` and email it to me by 11:30 PM on Thursday.


When you're finished, you should end up with a package directory structure similar to this:
```
catkin_ws
|__src
    |__chris_hw1
        |__ launch
           |__ chris_hw1.launch
        |__ src
           |__ chris_hw1.py.
        |__ other files/folders in pkg...
```

### TIPS
* Refer to the exercises; it's the same content, but applied to your own created package.
* All the info about packages (params, launch files, etc.) and ROS command syntax can be referred to on the [
ROS Wiki](http://wiki.ros.org/ROS/Tutorials)  
* Learn how to use the [bash terminal](https://www.youtube.com/watch?v=oxuRxtrO2Ag) (the black thing you type in). The more you know, the easier it gets, and the faster you can work.
* The majority of this HW will be spent debugging. Thus, a big component of this HW is practicing how to find the information you need to debug your error.
* Someone, somewhere at some point in time has run into any and every error you'll encounter and has found a solution. 
* Google is mankind's greatest invention. You may think you've been using its full potential, but I guarantee that you're not. So **Google how to Google effectively.**
