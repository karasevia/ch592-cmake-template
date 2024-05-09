target_sources(${TARGET_ELF} PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/broadcaster.c
    ${CMAKE_CURRENT_SOURCE_DIR}/devinfoservice.c
    ${CMAKE_CURRENT_SOURCE_DIR}/main.c
    ${CMAKE_CURRENT_SOURCE_DIR}/include/broadcaster.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/devinfoservice.h
)

target_include_directories(${TARGET_ELF} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)