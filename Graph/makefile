Graph: main.o Graph.o
	g++ main.o Graph.o -o Graph

main.o: main.cpp
	g++ -c main.cpp

Graph.o: Graph.cpp Graph.hpp
	g++ -c Interpreter.cpp

test: test.o
	g++ -std=c++11 test.o -o test

test.o: test.cpp
	g++ -c -std=c++11 test.cpp

maintest:
	./Graph < input.txt

clean:
	rm *.o test