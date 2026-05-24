add_executable(opengl-triangle)

target_sources(opengl-triangle
    PRIVATE
        main.cpp
)

# target_sources(opengl-triangle
#     PUBLIC
#         FILE_SET HEADERS
#         BASE_DIRS .
#         FILES
#         hello_triangle_application.hpp
#         opengl_validation.hpp
#         utilities.hpp
# )

# target_link_libraries(opengl-triangle PRIVATE Vulkan::Vulkan glfw glm::glm)

# Include the shader compilation module.
# list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/shaders/cmake")
# include(CompileShaders)
# add_shaders(opengl-triangle-shaders shaders/triangle.vert shaders/triangle.frag)


## TODO
#  - Learn more about install:
#    - install(TARGETS <name>
#      FILE_SET HEADERS
# )
#
# install(RUNTIME_DEPENDENCY_SET lib_deps
#  # Kolla CMAKE videon 2025...
# )

