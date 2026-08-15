# Data Structures and Algorithms Project: Database of Games

## Dataset Used
The dataset used is a slightly modified version of a public dataset provided on https://www.kaggle.com/datasets/sidtwr/videogames-sales-dataset. For reproducibility, name your dataset ```games_data.csv``` and place it in ```data/```

## Overview
This project is based around efficient storage and retrieval of data based on its structure, using the power of popular data structures. In a way, it is about building a customized highly efficient storage + retrieval API specifically designed to work for specific this specific data, to allow high speed searching, filtering and sorting. The dataset contains around 16.5k rows and 15 columns. During the storing progress, a significant amount of time is taken to store and organize the data in a very efficient manner to allow high functionality while keeping retrieval times to near instantaneous.

## Data Structures Usages
 
1	- **Graph** -	Storing each game's name, along with the list of games having the same name, within the program. Our graph has been implemented using an AVL tree data structure, where the games are sorted by name and where the nodes contain linked lists to store related games with the same name. O(log n) retrieval complexity.

2	- **Hash Table** - Storing all the games of a certain platform within a specific platform node within the hash table. O(1) retrieval complexity.

3 - **Hash Table** - Storing all the games of a certain genre within a specific genre node within the hash table. O(1) retrieval complexity.

4 - **Hash Table** - Storing all the games of a certain publisher within a specific publisher node within the hash table. O(1) retrieval complexity.

5 - **Hash Table** - Storing all the games of a certain developer within a specific developer node within the hash table. O(1) retrieval complexity.

6	- **Array** -	Storing all the games of a certain year within a specific year array node within the array. We have used an array because we can easily map the year to the node’s index within the array by subtracting 1980 (year of the oldest game in the dataset) from the year. O(1) retrieval complexity (because of year mapping).

7 - **Array** -	Storing all the games of a certain rating within a rating array node within the array. We have used an array because we can easily map the rating to the node’s index within the array, by using 8 if statements, as there are only 8 possible ratings. O(1) retrieval complexity (because the number of possible ratings is fixed).

8 - **AVL Tree** - To store the global sales data. Nodes are ranked by sales amount. Each node will have a linked list that contains all games that have the same global sales data. O(log n) retrieval complexity.

9 - **Doubly Linked Lists** - Doubly linked list is included at the nodes of some data structures. Multiple lists have been used to store games sorted by numeric data e.g. user score, user count, critic score, critic count etc. Doubly linked lists allow us to get data both in ascending and descending order. O(n) retrieval complexity.

## Demo
https://github.com/Hamaz-Hamza/Database-of-Games/assets/135416194/305de724-34a2-4afe-aec3-9e868202adcf
