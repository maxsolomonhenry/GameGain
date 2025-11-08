cmake_minimum_required(VERSION 3.22)

add_library(GameGainWwise STATIC
    SoundEnginePlugin/GameGainFX.cpp
    SoundEnginePlugin/GameGainFXParams.cpp
    SoundEnginePlugin/GameGainFXShared.cpp
)

target_compile_features(GameGainWwise PUBLIC cxx_std_17)

target_include_directories(GameGainWwise PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/SoundEnginePlugin
    ${WWISE_SDK_INCLUDE}
)
