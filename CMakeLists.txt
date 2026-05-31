cmake_minimum_required(VERSION 3.8)
project(system_interfaces)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(${PROJECT_NAME}
  "action/Find.action"
  "action/Scan.action"
  "action/Follow.action"
  "action/AssessScene.action"
  "action/ResolveTarget.action"
)

ament_package()
