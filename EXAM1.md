# EXAM 1
Covers all 3 HW assignments

## HW 1
**Unit 1: Guide for ROS in a Single Week
Unit 2: ROS Basics**

-   Creating a package with dependencies
-   Creating a Python Script
-   Creating and editing a launch file
-   Compiling `catkin_ws`

  

  

## HW 2 
**Unit 3: ROS Topics - Part 1**

**Git and Github**

-   Initializing a `.git` repo
-   Committing changes
-   Adding a remote Github repository
-   Pushing to a remote Github repository

  

**Messages**

-   Importing message types

e.g.: `from geometry_msgs.msg import Twist`

-   Identifying the structure of a message
-   Creating a custom message
-   Adding a custom message to `CMakeLists.txt`

  

**Publishers**

-   Creating a publisher node that publishes to a topic using the message type corresponding to that topic.

e.g. `pub = rospy.Publisher('/cmd_vel', Twist, queue_size=1)`

-   Publishing at a specific frequency

  

  

  

## HW 3 
**(Unit 4: ROS Topics - Part 2)**

**Subscribers**

-   Creating a subscriber node that subscribes to a topic of its corresponding message type, and invokes a callback function upon receiving a message to perform an action
-   Extracting data from individual components of a subscriber msg
