add_library(phy STATIC)

target_include_directories(phy PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

file(GLOB PHY_SOURCES "*.cpp")
if (NOT TARGET phy)
    add_library(phy
        phy.cpp
        phy_helpers.cpp
    )
endif()
