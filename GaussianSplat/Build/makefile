CFLAGS = -std=c++20
LDFLAGSLINUX = -lglfw -lGL -lX11 -lpthread -lXrandr -ldl
LDFLAGSWINDOWS = -lglfw3 -lopengl32 -lgdi32 -limm32 -lz

buildlinux:
	g++ $(CFLAGS) -I ../include -L ../lib -o opengl ../src/*.cpp ../src/*.c $(LDFLAGSLINUX)

buildwindows:
	g++ $(CFLAGS) -I ../include -L ../lib -o opengl ../src/*.cpp ../src/*.c $(LDFLAGSWINDOWS)

clean:
	rm opengl opengl.exe
