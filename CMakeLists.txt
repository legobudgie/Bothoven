#Minimum CMake required to build
cmake_minimum_required(VERISON 3.0)

#The project name
project(BotHoven)

#Set some compiler flags
add_definitions("-Wall" "-g")

#Set the include directory - for header files only!
include_directories({PROJECT_SOURCE_DIR}/include)

#Get all the source files in a specified subdirectory - requires re-run of cmake to collect new files
file(GLOB srcFiles src/.cpp)

#Add the main executable file
#!!!-If required for project is unkown-!!!
add_executable(BotHoven ${srcFiles})




