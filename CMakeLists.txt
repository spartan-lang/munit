project(Spartan C)

set(munit_SRCS munit.c munit.h)

add_library(munit STATIC ${munit_SRCS})

set_property(TARGET munit PROPERTY C_STANDARD 99)
set_property(TARGET munit PROPERTY C_STANDARD_REQUIRED ON)

target_include_directories(munit INTERFACE ${CMAKE_CURRENT_LIST_DIR})
