# Data Structures and Algorithms Project: Database of Games

## Dataset Used
The dataset used is a slightly modified version of a public dataset provided on https://www.kaggle.com/datasets/sidtwr/videogames-sales-dataset. For reproducibility, name your dataset ```games_data.csv``` and place it in ```data/```

## Introduction
This project is based around efficient storage and retrieval of data based on its structure, using the power of popular data structures. In a way, it is about building a customized highly efficient storage + retrieval API specifically designed to work for specific this specific data, to allow high speed searching, filtering and sorting. The dataset contains around 16720 rows and 15 columns, yet all operations are near instantaneous.

## Data Structures Usages

1	- **Graph** -	Storing the names and lists of related games for each game within the program. We have not used a hash table because hundreds of new games are added each year, so a hash table would not be efficient in this case. Our graph has O(log n) searching.

2	- **Hash Table** - Storing all the games of a certain platform within a specific platform node within the hash table. We have used a hash table to allow O(1) searching and retrieval.

3 - **Hash Table** - Storing all the games of a certain genre within a specific genre node within the hash table. We have used a hash table to allow O(1) searching and retrieval.

4 - **Hash Table** - Storing all the games of a certain publisher within a specific publisher node within the hash table. We have used a hash table to allow O(1) searching and retrieval.

5 - **Hash Table** - Storing all the games of a certain developer within a specific developer node within the hash table. We have used a hash table to allow O(1) searching and retrieval.

6	- **Array** -	Storing all the games of a certain year within a specific year array node within the array. We have used an array because we can easily map the year to the node’s index within the array by subtracting 1980 from the year.

7 - **Array** -	Storing all the games of a certain rating within a rating array node within the array. We have used an array because we can easily map the rating to the node’s index within the array, by using 8 if statements, as there are only 8 possible ratings.

8 - **AVL Tree** - To store the global sales data. Each node will have a linked list that contains all games that have the same global sales data. We have used an AVL tree to allow faster searching times.

9 - **Doubly Linked Lists** - A doubly linked list has been included in the above data structures. We have also used multiple lists to store games sorted by numeric data e.g. user score, user count, critic score, critic count etc. We have used a doubly linked list as it allows us to get data both in ascending and descending order


https://github.com/Hamaz-Hamza/Database-of-Games/assets/135416194/305de724-34a2-4afe-aec3-9e868202adcf
