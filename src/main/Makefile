OBJS=$(patsubst %.cpp,%.o,$(wildcard *.cpp))

include ../Mk/local.Mk
CXXINCLUDE+=-I./ -I../common  -I../models 
CXXINCLUDE+=-I/usr/local/include
# SEARCH 
CXXFLAGS+=-I../../../search2/src

all: $(OBJS) 

.cpp.o:
	$(CXX)  $(CXXFLAGS) $(CXXDEFINE) -c  $(CXXINCLUDE) $< 

.c.o:
	$(CXX)  $(FLAGS) $(CXXDEFINE) -c  $(CXXFLAGS) $(CXXINCLUDE) $< 

clean:
	$(RM) $(OBJS) *.moc $(UI_HEAD) $(UI_CPP)
