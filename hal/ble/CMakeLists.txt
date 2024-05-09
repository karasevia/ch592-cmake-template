target_sources(${TARGET_ELF} PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/ble_task_scheduler.S
    ${CMAKE_CURRENT_SOURCE_DIR}/CH59xBLE_LIB.h
)

target_include_directories(${TARGET_ELF} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})