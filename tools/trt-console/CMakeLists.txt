
file(GLOB trtConsoleSources *.cpp)
file(GLOB trtConsoleIncludes *.h )

cuda_add_executable(trt-console ${trtConsoleSources})
target_link_libraries(jetson-inference jetson-utils nvinfer nvinfer_plugin nvparsers)