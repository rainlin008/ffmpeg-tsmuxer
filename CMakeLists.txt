#
# @file CMakeLists.txt
# @author Akagi201
# @date 2014/11/18
#

cmake_minimum_required(VERSION 2.8.4)
project(ffmpeg_tsmuxer)

set(SOURCE_FILES main.c)

include_directories("/usr/local/include")

link_directories("/usr/local/lib")

add_executable(ffmpeg_tsmuxer ${SOURCE_FILES})

target_link_libraries(ffmpeg_tsmuxer "libavformat.a" "libavcodec.a" "libavutil.a")