CFLAGS= -std=c++20 -O2
LDFLAGS= -lglfw -lvulkan -ldl -lpthread -lX11 -lXxf86vm -lXrandr -lXi

all: VulkanTest

VulkanTest: main.cpp
	g++ $(CFLAGS) -o $@ main.cpp $(LDFLAGS)
