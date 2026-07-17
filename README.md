# WORMS Assets

## Setup

If you do not have xacro downloaded, you can do so with the following command:

```
sudo apt install ros-<ros2-distro>-xacro
```

## Compiling a WORM

The following command will compile a single WORM, fixed at the origin, with the pony namespace, and store it in the urdf folder.

```
ros2 run xacro xacro name:=pony xacro/3dof-worm.urdf.xacro > urdf/pony-worm.urdf
```

## Compiling a turtle pallet

The following command will compile a turtle pallet with worms of the indicated names, and store it in the urdf folder.

```
ros2 run xacro xacro \
        front_left:=duck \
        front_right:=frog \
        back_left:=lion \
        back_right:=pony \
    xacro/turtle.urdf.xacro > urdf/turtle.urdf
```
