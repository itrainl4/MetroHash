add_library(MetroHash
    STATIC
        src/metrohash.h
        src/platform.h
        src/metrohash64.h
        src/metrohash64.cpp
        src/metrohash128.h
        src/metrohash128.cpp
        src/metrohash128crc.h
        src/metrohash128crc.cpp
        src/testvector.h)

target_include_directories(MetroHash
    PUBLIC
        src)

set_target_properties(MetroHash
    PROPERTIES
        CXX_STANDARD          17
        CXX_STANDARD_REQUIRED ON)