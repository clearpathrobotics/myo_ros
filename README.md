# myo_ros

This serves as the ROS-side portion of what is required to get Myo to work on a ROS network. It currently only contains a few custom message definitions to keep the data coming into ROS as raw as possible, but some basic examples should be added to demonstrate how it can be used. The Windows-side portion is myo_ros_windows

## Installing Dependencies (Indigo)
    sudo apt-get install ros-indigo-rosserial-server

## Installing Dependencies (Hydro)
As of this writing, it has been untested in Hydro, but I see no reason why it wouldn't work.

    sudo apt-get install ros-hydro-rosserial-server

## Dependencies
Base ROS

## Compiling
Clone the source into your workspace and make your workspace. That's it.

## Running
As in the usual rosserial-based bridges, simply launch rosserial on this end:
    
    roslaunch rosserial_server socket.launch
You'll need to run the Windows side separately, consult the documentation for that package for those instructions.

## TODO:
Port previous example nodes to the new format to show Myo->ROS commands (ex. Twist)
