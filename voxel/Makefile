CXX=g++
CXXFLAGS=-std=c++11 -march=native -Ofast -Wall -Wextra -pedantic
LINKAGE=-lsfml-system -lsfml-graphics -lsfml-window -lGL $(shell pkg-config --cflags --libs glew)

SRC=main.cc voxelEngine.cc shader.cc camera.cc
BINARY=voxel

.PHONY: voxel

all: voxel

voxel:
	${CXX} ${CXXFLAGS} -o ${BINARY} ${SRC} ${LINKAGE}
