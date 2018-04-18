Minimal ROS package
-------------------

A ROS (Robot Operating System) package can contain anything else that logically constitutes a useful module, e.g. nodes, library, dataset, launch files. A minimal ROS package only needs to have a `package.xml`. This "minimal" package also includes a `CMakeLists.txt` and a C file `hello.c`.

#### To build the package

Suppose your ROS workspace is `catkin\_ws`. First be sure to set properly your environment variables. Usually, you source  catkin\_ws/devel/setup.sh to get things set.  Then clone this git repo into `catkin\_ws/src`. You can use catkin\_build to build all packages in catkin\_ws/src. You can also use this command to build only the `helloworld\_ros` package. 

 
```
$  catkin_build --pkg helloworld_ros
```

#### To run the program, do

```
$ ./devel/lib/helloworld_ros/hello
```

or

```
# rosrun helloworld_ros hello
```