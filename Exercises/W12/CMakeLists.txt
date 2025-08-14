# CMakeList.txt : CMake project for LMS, include source and define
# project specific logic here.
#

project(Project LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)

set(MODULE_DIRS People Content)

set(MODULE_LIBS "")

foreach(dir ${MODULE_DIRS})
    file(GLOB SRC_FILES ${dir}/*.cpp)
    add_library(${dir} ${SRC_FILES})
    target_include_directories(${dir} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/${dir})
    target_compile_features(${dir} PUBLIC cxx_std_20)

    list(APPEND MODULE_LIBS ${dir})
endforeach()

# Add source to this project's executable.
add_executable (LMS "LMS.cpp" "LMS.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET LMS PROPERTY CXX_STANDARD 20)
endif()

# Link các thư viện module vào executable
target_link_libraries(LMS PRIVATE ${MODULE_LIBS})

# TODO: Add tests and install targets if needed.
