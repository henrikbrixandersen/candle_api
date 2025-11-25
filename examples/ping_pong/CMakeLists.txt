project(ping_pong)

add_executable(${PROJECT_NAME} main.c)
include_directories(../../candle_api/include)
target_link_libraries(${PROJECT_NAME} ${CMAKE_SOURCE_DIR}/../candle_api/libcandle_api.a)
target_link_libraries(${PROJECT_NAME} ${CMAKE_SOURCE_DIR}/../candle_api/libusb-cmake/libusb-1.0.a)
target_link_libraries(${PROJECT_NAME} udev)
