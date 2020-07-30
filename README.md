# Moving_Obstacle_Gazebo
## For running the world
In a terminal (Source the files)

``` $ roslaunch husky_gazebo mowito_world.launch ```
## To edit the trajectory and velocity of moving obstacles
###  1)   For cube
#### Move to the file 
``` gazebo_world/src/gazebo/worlds/wall.world ```
#### From line 2487 to 2512.
##### To edit the trajectory, change the POSE values which are x,y coordinates in Lines (2493,2497,2501,2505,2509). 
##### To change the velocity of the moving obstacle change the TIME value in each waypoint in Lines (2492,2496,2500.2504,2508) .The time is in seconds, counted from the beginning of the script, when the pose should be reached.Higher the time the obstacles moves slowly.

###  2)   For SPHERE
##### Move to the file 
``` gazebo_world/src/gazebo/worlds/wall.world ```
#### From line 2408 to 2433.
##### To edit the trajectory, change the POSE values which are x,y coordinates in Lines (2414,2418,2422,2426,2430).
##### To change the velocity of the moving obstacle change the TIME value in each waypoint in Lines (2413,2417,2421,2425,2429).The time is in seconds, counted from the beginning of the script, when the pose should be reached.Higher the time the obstacles moves slowly.
