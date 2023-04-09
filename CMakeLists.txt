#cmake_minimum_required(VERSION 3.24)
#project(TinyCompiler C)
#
#set(CMAKE_C_STANDARD 11)
#
#add_executable(TinyCompiler main.c)

#cmake_minimum_required(VERSION 3.10)
#
#project(TinyCompiler C)
#
#add_executable(TinyCompiler ANALYZE.C CGEN.C CODE.C MAIN.C PARSE.C SCAN.C SYMTAB.C UTIL.C)
#
#set_target_properties(TinyCompiler PROPERTIES LINKER_LANGUAGE CXX)
#

cmake_minimum_required(VERSION 3.10)
project(TinyCompiler C)
# 解决 MSVC warning C4819

add_executable(Tiny analyze.c cgen.c code.c main.c parse.c scan.c symtab.c util.c)