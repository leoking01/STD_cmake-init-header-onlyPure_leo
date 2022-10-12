project(TestInstallation)
cmake_minimum_required(VERSION 3.5)

find_package(headeronly  REQUIRED  PATHS  "E:\\AAAAA_cmk_lib_export2\\cmake-init-header-onlyPure\\headeronly__install")

add_executable(mymathApp mymathApp.cc)
target_link_libraries(mymathApp headeronly::headeronly)
target_include_directories(mymathApp  PRIVATE  "E:\\AAAAA_cmk_lib_export2\\cmake-init-header-onlyPure\\headeronly__install/include/headeronly/headeronly")
