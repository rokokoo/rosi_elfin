# ROS Industrial - Elfin manipulator

## Cloning

Clone this repository, with it's submodules using the command

```bash
git clone --recurse-submodules https://github.com/rokokoo/rosi_elfin.git
```

Install required components, using the following command

```bash
rosdep install -yr --from-paths src --ignore-src
```

## Building

There is a build order error, in the `elfin_robot` package, so you need to run `catkin build` twice to get all the packages to compile.

```bash
catkin build; source devel/setup.bash; catkin build --unbuilt; source devel/setup.bash
```

## Visualize the model

To run the model in Gazebo

```bash
roslaunch samk_description gazebo.launch
```

To run the model in Rviz

```bash
roslaunch samk_description display.launch
```