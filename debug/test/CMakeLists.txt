include_directories (${CSGAMES_EXAM_2019_DEBUG_SOURCE_DIR}/src)

FILE(GLOB TEST_SOURCES *.cpp)

add_executable(karaoke_lib_test ${TEST_SOURCES})

target_link_libraries (karaoke_lib_test
        karaoke_lib
        Catch2::Catch2
        )