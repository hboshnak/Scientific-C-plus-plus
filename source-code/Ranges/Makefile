CXX = g++
CXXFLAGS = -std=c++14 -O2 -g -Wall -Wextra
CPPFLAGS = -I/usr/local/software/ranges/0.3.0/include
LDLIBS = -lm

all: transform_accumulate.exe

%.exe: %.o
	$(CXX) $(CXXFLAGS) $(CPPFLAGS) -o $@ $^ $(LDLIBS)

%.o: %.cpp
	$(CXX) $(CXXFLAGS) $(CPPFLAGS) -c -o $@ $<

clean:
	$(RM) *.exe *.o
	$(RM) core core.*
