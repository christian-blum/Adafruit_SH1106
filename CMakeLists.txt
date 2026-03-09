
cmake_minimum_required(VERSION 3.5)

idf_component_register(SRCS "Adafruit_SH1106.cpp"
                       INCLUDE_DIRS "."
                       REQUIRES arduino-esp32 Adafruit_BusIO Adafruit-GFX-Library)


target_compile_options(${COMPONENT_LIB} PRIVATE -Wno-deprecated-declarations)

project(Adafruit-SH1106)
