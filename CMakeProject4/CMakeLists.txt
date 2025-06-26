# CMakeList.txt : CMake project for CMakeProject4, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (CMakeProject4 "CMakeProject4.cpp" "CMakeProject4.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET CMakeProject4 PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
