# Makefile for Cyclone CUDA

# CUDA version and architecture settings
CUDA_VERSION ?= 12.9
CUDA_ARCH = sm_89

# Rules for building...

all: main

main: main.o
	$(NVCC) -o main main.o

main.o: main.cu
	$(NVCC) -c main.cu
