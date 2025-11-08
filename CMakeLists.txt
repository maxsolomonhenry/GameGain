cmake_minimum_required(VERSION 3.22)
project(GAME_GAIN VERSION 0.0.1)

set(WWISE_SDK_ROOT "/Applications/Audiokinetic/Wwise2024.1.9.8920/SDK")
set(WWISE_SDK_INCLUDE "${WWISE_SDK_ROOT}/include")
set(WWISE_SDK_LIB "${WWISE_SDK_ROOT}/Mac_Xcode1500/Release/lib")

add_subdirectory(JucePart)
add_subdirectory(WwisePart)