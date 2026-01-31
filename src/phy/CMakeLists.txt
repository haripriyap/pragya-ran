add_library(phy STATIC)

target_include_directories(phy PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

file(GLOB PHY_SOURCES "*.cpp")
add_library(phy ${PHY_SOURCES})
