cmake_minimum_required(VERSION 3.14.2)

project(BitWriter_2_9_func)


set(BitWriter_2_9_func_SRC_FILES
    BitcodeWriter.cpp                               
    BitcodeWriterPass.cpp
    ValueEnumerator.cpp
	)

include_directories(${CMAKE_SOURCE_DIR}/slang)

add_library(LLVMBitWriter_2_9_func STATIC ${BitWriter_2_9_func_SRC_FILES})

target_link_libraries(LLVMBitWriter_2_9_func)
