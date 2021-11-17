set(BUILD_SHARED_LIBS ON)

include(FetchContent_MakeAvailableExcludeFromAll)
include(FetchContent)
FetchContent_Declare(SDL2
    URL https://github.com/libsdl-org/SDL/archive/43d1b42a5ada15109409a8b448a753e25b3b1c1d.tar.gz
    URL_HASH MD5=e9df0145d0160eff65af4c566a709fbe
)
FetchContent_MakeAvailableExcludeFromAll(SDL2)

add_library(SDL2::SDL2 ALIAS SDL2)
