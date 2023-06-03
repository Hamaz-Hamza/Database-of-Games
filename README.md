Data Structures and Algorithms
Database of Games


An End-Semester Project by
Hamaz Hamza 365670
Omer Farooq 377187
Syed Hamza Ali Shah 396358


Introduction
In our project, we have made a program that stores data about games across many different years, genres, developers, platforms, etc. Our dataset includes 16720 rows and 15 columns. The data we have chosen also lists each game’s sales across the world, scores and user amounts by both critics and gamers. We have made 19 functions that allows the user to retrieve many different types of data from out dataset, and these will be described later. We have used graphs, AVL trees, doubly linked lists, arrays, and hash tables to store our data, these will be also be described later on.

Data Structures

1	- Graph -	Storing the names and lists of related games for each game within the program. We have not used a hash table because hundreds of new games are added each year, so a hash table would not be efficient in this case. Our graph has O(log n) searching.

2	- Hash Table - Storing all the games of a certain platform within a specific platform node within the hash table. We have used a hash table to allow O(1) searching and retrieval.

3 - Hash Table - Storing all the games of a certain genre within a specific genre node within the hash table. We have used a hash table to allow O(1) searching and retrieval.

4 - Hash Table - Storing all the games of a certain publisher within a specific publisher node within the hash table. We have used a hash table to allow O(1) searching and retrieval.

5 - Hash Table - Storing all the games of a certain developer within a specific developer node within the hash table. We have used a hash table to allow O(1) searching and retrieval.

6	- Array -	Storing all the games of a certain year within a specific year array node within the array. We have used an array because we can easily map the year to the node’s index within the array by subtracting 1980 from the year.

7 - Array -	Storing all the games of a certain rating within a rating array node within the array. We have used an array because we can easily map the rating to the node’s index within the array, by using 8 if statements, as there are only 8 possible ratings.

8 - AVL Tree - To store the global sales data. Each node will have a linked list that contains all games that have the same global sales data. We have used an AVL tree to allow faster searching times.

9 - Doubly Linked Lists - A doubly linked list has been included in the above data structures. We have also used multiple lists to store games sorted by numeric data e.g. user score, user count, critic score, critic count etc. We have used a doubly linked list as it allows us to get data both in ascending and descending order

