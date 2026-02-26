# unit2_teTernary Search (Divide and Conquer)

This program implements a ternary search algorithm in C++ to search for a song inside an alphabetically sorted playlist.

The idea behind ternary search is similar to binary search, but instead of dividing the list into two parts at each step, it divides the list into three parts. The algorithm compares the target value with two midpoint positions and then recursively searches the correct third of the list.

If the song is found, the program returns the index where it exists in the playlist. If it is not found, the program returns -1.

How to compile the program:

g++ ternary_search.cpp -o search

How to run the program after compiling:

./search

After running the program, you will be prompted to enter the name of a song. The program will then display whether the song was found and, if so, its index in the playlist.

Example:

Enter song to search: The Movie
Song found at index: 14

Time Complexity:

Each recursive call reduces the problem size to approximately n/3 while performing constant work.

Recurrence relation:
T(n) = T(n/3) + O(1)

This results in a time complexity of O(log n).

Binary search has recurrence:
T(n) = T(n/2) + O(1)

Binary search is also O(log n). Both algorithms are logarithmic, although binary search may require slightly fewer comparisons in practice.rnary_search
