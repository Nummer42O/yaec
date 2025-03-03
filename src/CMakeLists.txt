cmake_minimum_required(VERSION 3.16)


find_package(PkgConfig REQUIRED)
pkg_check_modules(
  GTKMM
  REQUIRED IMPORTED_TARGET
  gtkmm-3.0 glibmm-2.4
)


target_sources(mail-client
  PRIVATE
    main.cpp
)
add_subdirectory(3rd)
add_subdirectory(backend)
add_subdirectory(frontend)
