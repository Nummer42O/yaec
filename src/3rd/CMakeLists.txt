cmake_minimum_required(VERSION 3.16)


set(MAILIO_BUILD_DOCUMENTATION OFF)
set(MAILIO_BUILD_EXAMPLES OFF)
set(MAILIO_BUILD_TESTS OFF)
set(BUILD_SHARED_LIBS ON)
add_subdirectory(mailio)
target_link_libraries(mail-client
  PRIVATE
    mailio
)