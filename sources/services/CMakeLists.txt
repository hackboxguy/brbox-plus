cmake_minimum_required(VERSION 2.8.9)
set(PROJECT_NAME BrBoxServices)
project(${PROJECT_NAME})
add_subdirectory(sysmgr)
#add_subdirectory(smarteye)
add_subdirectory(gpioctl)
add_subdirectory(hotwire)
add_subdirectory(bboxsms)
add_subdirectory(xmproxy)
add_subdirectory(apisrv)


#for cross compiling
#cmake -H. -BOutput -DCMAKE_TOOLCHAIN_FILE=/path/to/toolchain-arm-backup.cmake -DCMAKE_INSTALL_PREFIX=/home/user/tmp/
#cmake --build Output -- all
#cmake --build Output -- install

#for local compiling
#cmake -H. -BOutput
#cmake --build Output -- all

#for cleaning make generated output
#rm -rf Output

