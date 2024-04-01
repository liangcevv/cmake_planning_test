cmake_minimum_required(VERSION 3.22.1)
project(planning)
set(CMAKE_CXX_STANDARD 17)

#变量和目录设置
#set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin) #动态库和exe都指定到bin目录下面
#set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
#CMAKE_ARCHIVE_OUTPUT_DIRECTORY
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
aux_source_directory(. SRC_LISTS)


#可执行文件
add_executable(planning_main ${SRC_LISTS})
