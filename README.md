# Concept-Of-Data-Science-
My Ternary Search Tree (TST) Implementation
Project Overview
This project is my Python implementation of a Ternary Search Tree (TST), which is an efficient data structure I built for storing and retrieving strings. I found it particularly useful for applications that require fast string search, insertion, and prefix matching, like dictionary lookups. In the context of my larger work, I designed it to manage DNA segments for sequence assembly.

Key Features
The TernarySearchTree class that I developed supports the following core operations:

insert(word): I implemented this to add a string to the tree.
search(word): I use this method to quickly check if a string exists in the tree.
__len__(): This returns the total number of unique strings I have stored.
traverse(): I designed this to retrieve all strings currently in the tree in alphabetical order.
How I Ran My Tests
I placed all test cases for my Ternary Search Tree implementation within the tst.ipynb Jupyter Notebook. These tests cover basic functionality, how it handles duplicates, edge cases like empty strings, and its performance when working with large datasets.

My tests utilize the following data files:

insert_words.txt: This file contains a list of words that I insert into the TST to verify correct insertion and search functionality.
not_insert_words.txt: This file contains words that I do not insert, and I use it to confirm that the search method correctly returns False for non-existent words.
corncob_lowercase.txt: This is a large dictionary file (over 50,000 words) that I use for stress-testing my TST's performance with a significant volume of data.
To run the tests yourself:

Make sure you have Jupyter Notebook installed (pip install notebook).
Place ternary_search_tree_module.py, tst.ipynb, insert_words.txt, not_insert_words.txt, and corncob_lowercase.txt in the same directory.
Open your terminal or command prompt, navigate to that directory, and run:
Bash

jupyter notebook
In the Jupyter interface that opens in your browser, click on tst.ipynb.
Run all cells within the notebook. The output will show the status of each test (✅ Passed or ❌ Failed).
Files I Included
ternary_search_tree_module.py: This is the Python script where I defined my TSTNode and TernarySearchTree classes.
tst.ipynb: This is the Jupyter Notebook containing all my test cases and examples of how to use the TST.
insert_words.txt: My test data for insertion.
not_insert_words.txt: My test data for searches of non-existent words.
corncob_lowercase.txt: The large dataset I used for performance testing.