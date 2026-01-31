add_library(mac STATIC)

target_include_directories(mac PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

file(GLOB MAC_SOURCES "*.cpp")
if (NOT TARGET mac)
    add_library(mac
        mac.cpp
        mac_helpers.cpp
    )
endif()


