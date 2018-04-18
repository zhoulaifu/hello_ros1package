Minimal ROS package
-------------------

A ROS (Robot Operating System) package can contain anything else that logically constitutes a useful module, e.g. nodes, library, dataset, launch files. A minimal ROS package only needs to have a `package.xml`.   This "minimal" package also includes a `CMakeLists.txt` and a C file `hello.c`. You could have used `catkin_create` to quickly create a new package with some bolierplate texts and file structures. 

#### How  to build

Suppose your ROS workspace is `catkin_ws`. First be sure to set properly your environment variables. Usually, you source  catkin\_ws/devel/setup.sh to get things set.  Then clone this git repo into `catkin_ws/src`. You can use `catkin_make`to build all packages in catkin_ws/src. You can also use this command to build only the `helloworld_ros` package. 

 
```
$  catkin_make --pkg helloworld_ros
```

#### How to run 

```
$ ./devel/lib/helloworld_ros/hello
```

or

```
# rosrun helloworld_ros hello
```
