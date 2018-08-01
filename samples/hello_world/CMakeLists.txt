
include($ENV{ZEPHYR_BASE}/cmake/app/boilerplate.cmake NO_POLICY_SCOPE)
project(NONE)

set (CMAKE_CXX_STANDARD 14)

target_sources(app PRIVATE src/main.cpp src/demo.cpp)

target_compile_options(app PRIVATE $<$<COMPILE_LANGUAGE:CXX>:-Wall -std=c++14>)
