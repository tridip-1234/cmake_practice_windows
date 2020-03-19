#set the minimum CMAKE version
cmake_minimum_required(VERSION 3.15.3)

#set the project name
project("tridip")

#add the executable
add_executable("${PROJECT_NAME}" "test1.cpp")

install(TARGETS "${PROJECT_NAME}" DESTINATION Build)  #$(CMAKE_INSTALL_PREFIX/bin)

install(FILES "test1.cpp" DESTINATION src)           #$(CMAKE_INSTALL_PREFIX/src)


#add_executable("${PROJECT_NAME}" "Main.cpp")

#install(TARGETS "${PROJECT_NAME}" DESTINATION bin)