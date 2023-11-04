
add_library(app1_lib STATIC app1.cpp)

add_executable(app1 main.cpp)

target_include_directories(app1_lib PRIVATE .)

target_link_libraries(app1 PUBLIC app1_lib module1_lib)
