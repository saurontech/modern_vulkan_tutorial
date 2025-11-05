CFLAGS= -std=c++20 -O2
LDFLAGS= -lglfw -lvulkan -ldl -lpthread -lX11 -lXxf86vm -lXrandr -lXi

all: VulkanTest slang.spv

VulkanTest: main.cpp slang.spv
	g++ $(CFLAGS) -o $@ main.cpp $(LDFLAGS)

slang.spv: shader.slang
	slangc ./shader.slang -target spirv -profile spirv_1_4 -emit-spirv-directly -fvk-use-entrypoint-name -entry vertMain -entry fragMain -o slang.spv

clean:
	rm ./VulkanTest ./slang.spv
