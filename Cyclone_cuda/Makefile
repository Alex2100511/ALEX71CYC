# Makefile for building the Cyclone CUDA Project

# Set CUDA architecture
CUDA_ARCH = sm_89
# Set source files
SRC = main.cu utils.cu
# Set output executable
OUTPUT = cyclone
# Set compiler
NVCC = nvcc
# Set compiler flags
NVCC_FLAGS = -arch $(CUDA_ARCH) -O3

# Define build targets
all: $(OUTPUT)

$(OUTPUT): $(SRC)
	$(NVCC) $(NVCC_FLAGS) -o $(OUTPUT) $(SRC)

clean:
	rm -f $(OUTPUT)