#设置cmake version
cmake_minimum_required(VERSION 3.17)
#设置变量名字
set(APP_NAME ConsoleDemo)
# 国际惯例 project name
project(${APP_NAME})
#C11
set(CMAKE_CXX_STANDARD 11)
# 这里需要链接静态库
link_libraries(${CMAKE_CURRENT_SOURCE_DIR}/libCmakeDemo.a)
#正常编译需要的 添加source 文件
add_executable(${APP_NAME} main.cpp library.h)
