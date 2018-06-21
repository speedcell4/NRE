cmake_minimum_required(VERSION 3.7)
project(project)

set(CMAKE_CXX_FLAGS "-O2 -lpthread")
set(CMAKE_CXX_STANDARD 11)

add_executable(cnn-att-train CNN+ATT/train.cpp CNN+ATT/init.h)
add_executable(cnn-att-test CNN+ATT/test.cpp CNN+ATT/test.h CNN+ATT/init.h)

add_executable(cnn-one-train CNN+ONE/train.cpp CNN+ONE/init.h)
add_executable(cnn-one-test CNN+ONE/test.cpp CNN+ONE/test.h CNN+ONE/init.h)

add_executable(pcnn-att-train PCNN+ATT/train.cpp PCNN+ATT/init.h)
add_executable(pcnn-att-test PCNN+ATT/test.cpp PCNN+ATT/test.h PCNN+ATT/init.h)

add_executable(pcnn-one-train PCNN+ONE/train.cpp PCNN+ONE/init.h)
add_executable(pcnn-one-test PCNN+ONE/test.cpp PCNN+ONE/test.h PCNN+ONE/init.h)