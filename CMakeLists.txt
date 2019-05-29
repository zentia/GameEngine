#1.cmake version,指定cmake版本
cmake_minimum_required(VERSION 2.6)
#2.指定项目名称，一般和项目的文件夹名对应
project(GameEngine)
#3.头文件目录
INCLUDE_DIRECTORIES(
	./inc
)
#4.源文件目录
SET(SOURCE_FILES
./main.cpp)
SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin) # 设置可执行文件的输出目录
ADD_EXECUTABLE("GameEngine" ${SOURCE_FILES})