Graph: main.o Graph.o
	g++ main.o Graph.o -o Graph

main.o: main.cpp
	g++ -c main.cpp

Graph.o: Graph.cpp Graph.hpp
	g++ -c Interpreter.cpp

test: tests.o
	g++ -std=c++11 tests.o -o test

tests.o: tests.cpp
	g++ -c -std=c++11 tests.cpp

maintest:
	./Graph < input.txt

clean:
	rm *.o test