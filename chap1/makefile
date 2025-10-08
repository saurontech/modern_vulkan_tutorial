CFLAGS= -std=c++17 -O2
LDFLAGS= -lglfw -lvulkan -ldl -lpthread -lX11 -lXxf86vm -lXrandr -lXi

all: VulkanTest

VulkanTest: main.cpp
	g++ $(CFLAGS) -o $@ main.cpp $(LDFLAGS)
