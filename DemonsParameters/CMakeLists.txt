# This is the root ITK CMakeLists file.
cmake_minimum_required(VERSION 2.4)
if(COMMAND CMAKE_POLICY)
  cmake_policy(SET CMP0003 NEW)
endif()


# This project is designed to be built outside the Insight source tree.
project(Demons)

# Find ITK.
find_package(ITK REQUIRED)
include(${ITK_USE_FILE})

find_package(VTK)
if(VTK_FOUND)
	include(${USE_VTK_FILE})
endif(VTK_FOUND)

add_executable(Demons DeformableRegistration2.cxx )

target_link_libraries(Demons ${ITK_LIBRARIES})
