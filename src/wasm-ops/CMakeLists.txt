set(SGEMM_SOURCES
  matmul.cpp
  utils/broadcast_utils.cpp
  utils/shape_utils.cpp)

add_library(onxx-sgemm STATIC ${SGEMM_SOURCES})
target_include_directories(onxx-sgemm PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
