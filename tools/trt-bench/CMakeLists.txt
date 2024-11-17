
file(GLOB trtBenchSources *.cpp)
file(GLOB trtBenchIncludes *.h )

cuda_add_executable(trt-bench ${trtBenchSources})
target_link_libraries(jetson-inference jetson-utils nvinfer nvinfer_plugin nvparsers)
