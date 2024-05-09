add_subdirectory(ble)
#add_subdirectory(flash)
add_subdirectory(StdPeriphDriver)

target_sources(${TARGET_ELF} PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/startup_CH592.S
    ${CMAKE_CURRENT_SOURCE_DIR}/KEY.c
    ${CMAKE_CURRENT_SOURCE_DIR}/LED.c
    ${CMAKE_CURRENT_SOURCE_DIR}/MCU.c
    ${CMAKE_CURRENT_SOURCE_DIR}/RTC.c
    ${CMAKE_CURRENT_SOURCE_DIR}/SLEEP.c
    ${CMAKE_CURRENT_SOURCE_DIR}/include/CONFIG.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/HAL.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/KEY.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/LED.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/RTC.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/SLEEP.h
)

target_include_directories(${TARGET_ELF} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)