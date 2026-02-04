target_sources_ifdef(CONFIG_ZMK_BEHAVIOUR_OS_LAYER app PRIVATE src/behaviour_os_layer.c)

if(CONFIG_ZMK_INPUT_PROCESSOR_SCROLL_ACCELERATION)
    zephyr_library_named(zmk-input-processor-scroll-acceleration)
    zephyr_library_sources(src/input_processor_scroll_acceleration.c)
endif()