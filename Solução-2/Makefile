CXX       = g++
CXXFLAGS  = -Wall -I.

PROGRAM   = virusim
SRCS      = virusim.cpp Random.cpp Population.cpp
OBJS      = $(SRCS:.cpp=.o)

.SUFFIXES: .cpp .o

.cpp.o:
	$(CXX) -c $(CXXFLAGS) $<

all:
	$(CXX) -fopenmp -o $(PROGRAM) $(SRCS) $(CXXFLAGS) $(LDFLAGS)

clean:
	/bin/rm -f $(OBJS) $(PROGRAM)
