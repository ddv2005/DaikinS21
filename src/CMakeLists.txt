set (COMPONENT_SRCS "Faikin.c" "ela.c")
set (COMPONENT_REQUIRES "ESP32-RevK" "espressif__mdns")
register_component ()
target_add_binary_data(${COMPONENT_TARGET} "apple-touch-icon.png" BINARY)