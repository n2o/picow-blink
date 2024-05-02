cmake_minimum_required(VERSION 3.13)

include(pico_sdk_import.cmake)

project(blink)

pico_sdk_init()

add_executable(blink
        blink.c
)

# Add pico_stdlib library which aggregates commonly used features
target_link_libraries(blink pico_stdlib pico_cyw43_arch_none)

# create map/bin/hex/uf2 file in addition to ELF.
pico_add_extra_outputs(blink)