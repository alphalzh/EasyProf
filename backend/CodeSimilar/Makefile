CXX = g++
PROJECT = codeS
OBJECTS = main.o
#TEST_PROJECT = lockAnalysis_test
#TEST_OBJECTS = ct_event_mock.o LockAnalysis.o lockAnalysis_test.o 
CPPFLAGS  = -O3 -g --std=c++11
LIBS = -lct_event -L../../common/eventLib/ -L../../common/taskLib/ -lTask -lz -Wl,-rpath=$(CONTECH_HOME)/common/taskLib/

all: $(PROJECT)

$(PROJECT): $(OBJECTS)
	$(CXX) $(OBJECTS) $(LIBS) -o $(PROJECT) 

#ct_event_mock.o:
#	$(CXX) -O3 -g -c -o ct_event_mock.o ct_event_mock.c

#test: $(TEST_OBJECTS)
#	$(CXX) $(TEST_OBJECTS) -o $(TEST_PROJECT)
#	./lockAnalysis_test

clean:
	rm -f $(PROJECT) $(OBJECTS)
#	rm -f $(TEST_PROJECT) $(TEST_OBJECTS)

	
