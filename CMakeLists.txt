cmake_minimum_required(VERSION 2.8.3)

project(slam_bot)

add_compile_options(-std=c++11)

find_package(catkin REQUIRED)

catkin_package()

find_package(roslaunch)

find_package(catkin REQUIRED COMPONENTS
    message_generation
    geometry_msgs
    std_msgs
    actionlib
    move_base_msgs
    roscpp
)

foreach(dir config launch meshes urdf)
	install(DIRECTORY ${dir}/
		DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach(dir)

include_directories(
    include
    ${catkin_INCLUDE_DIRS}
)

add_executable(navigation_goal src/navigation_goal.cpp)

target_link_libraries(navigation_goal ${catkin_LIBRARIES})


