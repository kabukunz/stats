# CMakeLists.txt

cmake_minimum_required(VERSION 2.8)

# cc / cxx
project(rtsc cxx)

# cmake a là make

# -I
include_directories(/Users/max/Developer/Library/Graphics/trimesh2/include)

# -L
link_directories(/Users/max/Developer/Library/Graphics/trimesh2/lib.Darwin64)

# -l
link_libraries(libtrimesh.a)
link_libraries(libgluit.a)

# cc
add_executable(rtsc rtsc.cc apparentridge.cc)