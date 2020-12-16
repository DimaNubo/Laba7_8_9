file(GLOB hdrs "*.h*")
file(GLOB srcs "*.cpp")

include_directories("${CMAKE_CURRENT_SOURCE_DIR}/../gtest")

add_executable(${ListTest} ${srcs} ${hdrs})
target_link_libraries(${ListTest} ${ListLib} gtest)