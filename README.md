# My DNA Sequence Assembly Project with Ternary Search Trees

Welcome to my repository for the "DNA Sequence Assembly" project, developed as part of my Advanced Programming in Python course. This repository showcases my implementation of a Ternary Search Tree (TST) and its application in efficiently managing and assembling DNA sequences. I've focused on creating a robust and performant solution, including a thorough analysis of its time complexity and real-world performance on high-performance computing resources.

## Project Overview

In this project, I've developed a Python-based system for DNA sequence assembly. The core of my solution relies on a custom-built Ternary Search Tree (TST) data structure. I chose the TST for its efficiency in handling string operations, which are crucial for searching, inserting, and finding prefixes of DNA segments during the assembly process. My aim was to reconstruct a complete DNA sequence from smaller, overlapping segments, and the TST proved to be an excellent tool for this task.

## Key Features

The `TernarySearchTree` class that I developed supports the following essential string operations:

* **`insert(word)`**: I implemented this method to efficiently add a new DNA segment (string) to the tree.
* **`search(word)`**: I use this to quickly check if a specific DNA segment already exists within the tree.
* **`__len__()`**: This property allows me to easily get the total count of unique DNA segments I have stored in the tree.
* **`traverse()`**: I designed this to retrieve all stored DNA segments in alphabetical order, which can be useful for debugging or inspection.

## Performance Analysis & Results

I extensively analyzed the performance of my Ternary Search Tree implementation to understand its efficiency and scalability.

* I generated a **time complexity graph** (`time_complexity_graph.png`) to visually illustrate how the TST's performance scales with increasing input sizes (number of words and word lengths). This graph clearly demonstrates the TST's efficiency characteristics.
* Furthermore, I obtained **supercomputing output results** (`supercomputing_results.log`) from running my TST on high-performance computing resources. These results allowed me to rigorously assess its performance and scalability under demanding conditions, particularly when handling very large datasets like `corncob_lowercase.txt`.

## How I Ran My Tests

All the test cases for my Ternary Search Tree implementation are meticulously documented and executed within the `tst.ipynb` Jupyter Notebook. These tests cover a wide range of scenarios, including basic functionality, handling of duplicate insertions, edge cases (like empty strings), and validating performance with large datasets.

My tests utilize the following data files:

* `insert_words.txt`: This file contains a list of words that I use for verifying the correct insertion and search functionality of the TST.
* `not_insert_words.txt`: This file holds words that I purposely do *not* insert. I use them to confirm that the `search` method correctly returns `False` for non-existent words.
* `corncob_lowercase.txt`: This is a very large dictionary file (over 50,000 words) that I leverage for robust stress-testing and evaluating the TST's performance under heavy load.

**To run the tests yourself:**

1.  Make sure you have Jupyter Notebook installed (`pip install notebook`).
2.  Clone this repository to your local machine:
    ```bash
    git clone [https://github.com/Rakshith234/Concept-Of-Data-Science-.git](https://github.com/Rakshith234/Concept-Of-Data-Science-.git)
    cd Concept-Of-Data-Science-
    ```
3.  Ensure all necessary files (`ternary_search_tree_module.py`, `tst.ipynb`, `insert_words.txt`, `not_insert_words.txt`, and `corncob_lowercase.txt`) are in the same directory.
4.  Open your terminal or command prompt, navigate to the cloned repository's directory, and launch Jupyter:
    ```bash
    jupyter notebook
    ```
5.  In the Jupyter interface that opens in your browser, click on `tst.ipynb`.
6.  Run all cells within the notebook (`Cell -> Run All`). The output will display the status of each test (`✅ Passed` or `❌ Failed`).

## Repository Contents

Here’s a breakdown of the files I’ve included in this repository:

* `ternary_search_tree_module.py`: This is the core Python script where I defined my `TSTNode` class (the building block of the TST) and the `TernarySearchTree` class with all its methods.
* `tst.ipynb`: This is my Jupyter Notebook. It contains all the test cases for the TST, demonstrations of its usage, and the code I used to generate the time complexity graph.
* `insert_words.txt`: My test data file containing words specifically for insertion tests.
* `not_insert_words.txt`: My test data file containing words to verify negative search results.
* `corncob_lowercase.txt`: The large dictionary file I used for extensive performance testing.
* `time_complexity_graph.png`: An image file presenting the visual representation of my TST's time complexity.
* `supercomputing_results.log`: A log file containing the detailed output and results from my supercomputing runs, demonstrating the TST's performance on high-end hardware.
* `project_appy.pdf`, `project_appy-2.pdf`: These are the original project assignment documents detailing the requirements and expectations for the DNA Sequence Assembly project.
* `output_1.png`: An example image, likely a screenshot of output related to DNA sequence assembly, as provided in the project specifications.

## Summary of My Conclusions

Through this project, I've drawn several key conclusions about the Ternary Search Tree and its application to DNA sequence assembly:

1.  **Efficiency of TST:** My implementation of the Ternary Search Tree proved to be a highly efficient data structure for string-based operations. Its design, leveraging character comparisons to traverse through `left`, `middle`, and `right` child nodes, enabled very fast insertion and search times, especially crucial for handling numerous DNA segments.
2.  **Scalability for Large Datasets:** The performance analysis, particularly with the `corncob_lowercase.txt` dataset and the supercomputing output, confirmed the TST's robust scalability. It maintained good performance characteristics even with tens of thousands of strings, indicating its suitability for real-world biological datasets which can be vast.
3.  **Applicability to DNA Assembly:** The TST's ability to perform efficient prefix searches and store varying length strings makes it an excellent choice for DNA sequence assembly. While the full assembly logic would reside in `project.py`, the TST provides the underlying backbone for quick lookups of overlapping segments, which is a critical step in reconstructing longer DNA sequences.
4.  **Reproducibility:** My detailed test cases in `tst.ipynb` and documented code demonstrate that the TST implementation is robust and its behavior is predictable, allowing for easy verification and future development. The inclusion of the time complexity graph and supercomputing logs further enhances the reproducibility and transparency of my performance claims.