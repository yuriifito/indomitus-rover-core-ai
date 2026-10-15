cmake_minimum_required(VERSION 3.5)
project(rover_navigation)

find_package(ament_cmake REQUIRED)

# Install launch, config, and behavior tree directories
install(DIRECTORY launch config behaviour_trees resource
    DESTINATION share/${PROJECT_NAME}
)

ament_package()