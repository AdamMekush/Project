add_executable(Project main.cpp)

target_include_directories(Project PRIVATE
  ${CMAKE_SOURCE_DIR}/src
  ${CMAKE_SOURCE_DIR}/include
 )

target_link_libraries(Project libcurl)
target_link_libraries(Project nlohmann_json)