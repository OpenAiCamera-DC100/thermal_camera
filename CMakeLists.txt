cmake_minimum_required(VERSION 3.8)

project(thermal_camera)

set(INFIRAY_LIB
    ${CMAKE_SOURCE_DIR}/lib/libUSBSDK.so
    ${CMAKE_SOURCE_DIR}/lib/libUSBSDK.so.1
    ${CMAKE_SOURCE_DIR}/lib/libUSBSDK.so.1.0
    ${CMAKE_SOURCE_DIR}/lib/libUSBSDK.so.1.0.0
)

install(FILES ${INFIRAY_LIB} DESTINATION lib)
install(DIRECTORY ${CMAKE_SOURCE_DIR}/include/ DESTINATION "include")
