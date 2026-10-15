cmake_minimum_required(VERSION 3.5)
project(rover_sensors)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY launch config resource
  DESTINATION share/${PROJECT_NAME}
)

install(
  DIRECTORY docs
  DESTINATION share/${PROJECT_NAME}
  OPTIONAL
)

install(
  FILES README.md
  DESTINATION share/${PROJECT_NAME}
  OPTIONAL
)

ament_package()
