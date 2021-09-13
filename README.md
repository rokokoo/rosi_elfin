# ROS Industrial - Elfin manipulator

## Cloning

Clone this repository, with it's submodules using the command

```bash
git clone --recurse-submodules https://github.com/rokokoo/rosi_elfin.git
```

## Building

There is a build order error, in the `elfin_robot` package, so you need to run `catkin build` twice to get all the packages to compile.

```bash
catkin build; source devel/setup.bash; catkin build --unbuilt; source devel/setup.bash
```

