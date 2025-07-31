cmake_minimum_required(VERSION 2.8.3)
project(robotiq_85_driver)

## Uncomment if the package has a setup.py
catkin_python_setup()

find_package(catkin REQUIRED COMPONENTS roslaunch rospy)

catkin_package()

catkin_install_python(PROGRAMS 
  src/robotiq_85/robotiq_85_driver.py
  src/robotiq_85/robotiq_85_gripper_test.py
  src/robotiq_85/robotiq_85_gripper.py
  src/robotiq_85/gripper_io.py
  src/robotiq_85/modbus_crc.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
                      
