# 设置需要编译的源文件列表
set(SRC_LIST ./muduo_server.cpp)

# 设置可执行文件最终存储的路径
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
add_executable(server ${SRC_LIST})
target_link_libraries(server muduo_net muduo_base pthread)