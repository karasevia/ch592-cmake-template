target_sources(${TARGET_ELF} PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/flash_info.c
    ${CMAKE_CURRENT_SOURCE_DIR}/internal_flash.c
    ${CMAKE_CURRENT_SOURCE_DIR}/spi_flash.c
    ${CMAKE_CURRENT_SOURCE_DIR}/include/flash_info.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/internal_flash.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/spi_flash.h
)

target_include_directories(${TARGET_ELF} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)