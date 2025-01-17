# Main executables
set(target_name das)

add_executable(${target_name} das.cpp)
set_target_properties(${target_name} PROPERTIES RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}")
