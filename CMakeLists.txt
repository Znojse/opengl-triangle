cmake_minimum_required(VERSION 3.29)
project(opengl-triangle VERSION 0.0.1 LANGUAGES C CXX)

find_package(Catch2 REQUIRED)

include(GNUInstallDirs)

if (${ENABLE_LINT})
    set(CMAKE_CXX_CLANG_TIDY
        clang-tidy;
        -p=${CMAKE_BINARY_DIR};
        -config-file=${CMAKE_SOURCE_DIR}/.clang-tidy;
        --quiet
    )
endif()

add_subdirectory(src)
# add_subdirectory(test)
