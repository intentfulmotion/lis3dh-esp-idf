cmake_minimum_required(VERSION 3.5)

set(srcs "src/esp_wrapper.c" "src/lis3dh.c")

idf_component_register(
  SRCS "${srcs}" 
  INCLUDE_DIRS "src" 
  REQUIRES soc)
