CMAKE_MINIMUM_REQUIRED(VERSION 2.8.4)
PROJECT(hello)
SET(MY_NAME 123)
MESSAGE(${MY_NAME})
MESSAGE("ADD_SUBDIRECTORY 用于多目录结构工程下，包含子目录,调用子目录的cmake文件")
MESSAGE("第一个参数为目录名称，第二个参数为生成目标文件的路径，在build目录下创建该目录")
ADD_SUBDIRECTORY(lib lib)
ADD_SUBDIRECTORY(src bin)

