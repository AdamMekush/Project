add_executable(Project main.cpp main.h)
target_link_libraries(Project libcurl)
target_link_libraries(Project nlohmann_json)