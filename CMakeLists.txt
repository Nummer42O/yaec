cmake_minimum_required(VERSION 3.16)
project(yaec
  VERSION 0.0.0
  DESCRIPTION "Yet Another Email Client (YÆC) is a small, lightweight GTK Email client meant for the Gnome desktop environment."
  HOMEPAGE_URL "https://github.com/Nummer42O/yaec"
  LANGUAGES CXX
)


include(GNUInstallDirs)


add_executable(mail-client)
add_subdirectory(src)


# TODO:
# - configure files?
# - options?
# - install target
# - uninstall target
