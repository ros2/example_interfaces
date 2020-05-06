cmake_minimum_required(VERSION 3.5)

project(example_interfaces)

# Default to C++14
if(NOT CMAKE_CXX_STANDARD)
  set(CMAKE_CXX_STANDARD 14)
endif()
if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(${PROJECT_NAME}
  "action/Fibonacci.action"
  "msg/Bool.msg"
  "msg/Byte.msg"
  "msg/Char.msg"
  "msg/Empty.msg"
  "msg/Float32.msg"
  "msg/Float64.msg"
  "msg/Int8.msg"
  "msg/Int16.msg"
  "msg/Int32.msg"
  "msg/Int64.msg"
  "msg/String.msg"
  "msg/UInt8.msg"
  "msg/UInt16.msg"
  "msg/UInt32.msg"
  "msg/UInt64.msg"
  "msg/WString.msg"
  "srv/AddTwoInts.srv"
  "srv/SetBool.srv"
  "srv/Trigger.srv"
)

install(FILES mapping_rules.yaml DESTINATION share/${PROJECT_NAME})

ament_export_dependencies(rosidl_default_runtime)
ament_package()
