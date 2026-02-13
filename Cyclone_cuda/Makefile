# Makefile for building Cyclone project

# Compiler settings
CC = nvcc

# Architecture settings for RTX 5060
TARGET_ARCH = sm_89

# Source files
SRC = main.cu helper.cu

# Output binary
OUTPUT = cyclone

# Build target
all: $(OUTPUT)

$(OUTPUT): $(SRC)
	$(CC) -arch $(TARGET_ARCH) $(SRC) -o $(OUTPUT)

clean:
	rm -f $(OUTPUT) *.o
