add_library(mac STATIC)

target_include_directories(mac PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

file(GLOB MAC_SOURCES "*.cpp")
add_library(mac ${MAC_SOURCES})


