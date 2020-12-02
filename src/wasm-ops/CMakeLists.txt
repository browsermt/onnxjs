set(SGEMM_SOURCES
  matmul.cpp
  utils/broadcast_utils.cpp
  utils/shape_utils.cpp)

add_library(onnx-sgemm STATIC ${SGEMM_SOURCES})
target_include_directories(onnx-sgemm PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
