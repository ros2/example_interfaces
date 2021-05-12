^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package example_interfaces
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Forthcoming
-----------

0.9.2 (2021-04-06)
------------------
* Change links from index.ros.org -> docs.ros.org. (`#13 <https://github.com/ros2/example_interfaces/issues/13>`_)
* Contributors: Chris Lalancette

0.9.1 (2021-03-18)
------------------
* Update maintainer (`#12 <https://github.com/ros2/example_interfaces/issues/12>`_)
* Contributors: Jacob Perron

0.9.0 (2020-05-26)
------------------
* Merge pull request `#11 <https://github.com/ros2/example_interfaces/issues/11>`_ from ros2/migrate_std_msgs
  Migrate content from std_msgs
* language cleanups from review
* remove duplicate message declarations
* Port MultiArray messages with warnings about being examples
* add generation flags for missed datatypes
* remove ColorRGBA which is still used from std_msgs
* Fill in CMake for msgs and add comments about status
* Integrate srv generation and add comments
* copy over std_msgs
* Contributors: Tully Foote

0.8.0 (2020-04-30)
------------------
* Merge pull request `#9 <https://github.com/ros2/example_interfaces/issues/9>`_ from ros2/claire/update-tutorial-link
  update tutorial link
* update tutorial link
* add mapping for rospy_tutorials/AddTwoInts.srv (`#7 <https://github.com/ros2/example_interfaces/issues/7>`_)
* Contributors: Claire Wang, Dirk Thomas

0.7.1 (2019-05-29)
------------------
* Remove the action_msgs dependency CMake code. (`#6 <https://github.com/ros2/example_interfaces/issues/6>`_)
  It is implicitly added by rosidl_generate_interfaces().
* Contributors: Jacob Perron

0.7.0 (2019-04-14)
------------------
* add section about DCO to CONTRIBUTING.md
* Contributors: Dirk Thomas

0.6.2 (2019-02-08)
------------------
* Remove action mapping for ROS 1 (`#5 <https://github.com/ros2/example_interfaces/issues/5>`_)
  Removing until this feature is supported by the bridge.
* Contributors: Jacob Perron

0.6.1 (2018-12-06)
------------------
* Add Fibonacci.action (`#4 <https://github.com/ros2/example_interfaces/issues/4>`_)
  * Add Fibonacci action
  Also added mapping rules for the Fibonacci action from ROS 1.
* Contributors: Jacob Perron

0.6.0 (2018-11-19)
------------------
* use add_compile_options instead of setting only cxx flags
* Contributors: Mikael Arguedas

0.5.0 (2018-06-25)
------------------
* advise to ask questions on ROS answers
* Contributors: Mikael Arguedas

0.4.0 (2017-12-08)
------------------
* member of rosidl_interfaces_packages group (`#2 <https://github.com/ros2/example_interfaces/issues/2>`_)
  * member of rosidl_interfaces_packages group
  * rosidl_interfaces_packages -> rosidl_interface_packages
* 0.0.3
* add issue template
* 0.0.2
* use CMAKE_X_STANDARD and check compiler rather than platform
* restore contrib, license, and readme after moving
* add pedantic flag
* Revert "readd dummy message" (`#163 <https://github.com/ros2/example_interfaces/issues/163>`_)
* Comment mapping_rules.yaml (`#156 <https://github.com/ros2/example_interfaces/issues/156>`_)
* Merge pull request `#155 <https://github.com/ros2/example_interfaces/issues/155>`_ from ros2/readd_msg
  readd dummy message
* readd dummy message to workaround `#154 <https://github.com/ros2/example_interfaces/issues/154>`_
* Messages and services mappings moved to one file
* Cpp14 (`#147 <https://github.com/ros2/example_interfaces/issues/147>`_)
  move to C++14 and use standard duration literals
* Merge pull request `#136 <https://github.com/ros2/example_interfaces/issues/136>`_ from haueck/service_mapping_rules
  Added a service mapping rule
* remove unused LargeFixed msg (`#150 <https://github.com/ros2/example_interfaces/issues/150>`_)
  * remove unused LargeFixed msg
  * remove builtin_interfaces from dependencies
* Added a service mapping rule
  It enables ros1_bridge to connect the AddTwoInts service
  from this package with the TwoInts from ros/roscpp_tutorials.
* update schema url
* add schema to manifest files
* require CMake 3.5
* Example of using MessagePoolMemoryStrategy
* add explicit build type
* raise warning level
* major refactor of examples and message packages
  builtin_msgs was moved to the common_interfaces
  repository and renamed builtin_interfaces.
  simple_msgs was also moved to common_interfaces
  and it was renamed std_interfaces.
  userland_msgs was renamed example_interfaces.
  userland was pruned and divided into
  rclcpp_examples and rclc_examples.
  There is a 'pre_refactor' tag that was made
  just before this commit.
* Contributors: Dirk Thomas, Jackie Kay, Mikael Arguedas, Morgan Quigley, Rafal Kozik, William Woodall, dhood
