# Project Title

### Memory-Management-using-Splay-trees

## Getting Started
This Project demonstrates the memory management operation in GCC compiler using the Splay tree data structure.Splay tree is an efficient data strture to store the static data in the memory and implements the concept of Region of Interest (ROI) which helps to find the last accessed nodes in minimal time as they are placed in locations near the ROOT of tree.

### Prerequisites

Platform used is Netbeans IDE 8.2
You can get it free from:   [Netbeans Download](https://netbeans.org/downloads/)
```
Basic JAVA programming.
Splay tree standard algorithms.
```
### Splay tree SPLAY operation

```
Search Operation
The search operation in Splay tree does the standard BST search, in addition to search, it also splays (move a node to the root).
If the search is successful, then the node that is found is splayed and becomes the new root. 
Else the last node accessed prior to reaching the NULL is splayed and becomes the new root.
```

### Splay tree INSERT Operation
```
The insert operation is similar to Binary Search Tree insert with additional steps to make sure that the newly inserted key becomes the new root.
Following are different cases to insert a key k in splay tree.
1) Root is NULL: We simply allocate a new node and return it as root.
2) Splay the given key k. If k is already present, then it becomes the new root. If not present, then last accessed leaf node becomes the new root.
3) If new root’s key is same as k, don’t do anything as k is already present.
4) Else allocate memory for new node and compare root’s key with k.
    4.a) If k is smaller than root’s key, make root as right child of new node, copy left child of root as left child of new node and make left child of root as NULL.
    4.b) If k is greater than root’s key, make root as left child of new node, copy right child of root as right child of new node and make right child of root as NULL.
5) Return new node as new root of tree.
```

### Memory management
1. Every node in the Tree consists of (key,value) pair, where key=Scope of Varaible and value=Value of varaible
2. Everytime we access the new symbol it is inserted in the tree, and splayed to the ROOT of tree.
3. If the accessed varaible already exists in the tree, we search in the tree and splay the key to ROOT.

## Running the File

Open the Source file Splay_Trees.java and Run it. 

### Importing the Project
```
1. Download the ZIP file for Project
2. Open Netbeans IDE and Go to File menu and Select Import Project
3. Choose "Import from ZIP", and search for the location where you saved the downloaded ZIP file
4. Choose the file and then let it load the project.
5. Open the  Splay_Trees.java file and run the file using "Shift+F6" or right click anywhere in the Code pane and choose option to Run file.
```
## Versioning

This is basic version of the Project. I will add more sophiscated Application version soon in the future.

## Features to be added

```
* Parsing the tokens using JAVA PARSER CC
* Recursive Functions call tracing

```

## Author

* **Rakshit Kathawate** - *Initial work* - [ChampionTej05](https://github.com/ChampionTej05)

## License

This project is not licensed. You can use this, for study purposes. For any commercial or promotive purposes, permission should be taken from Author,

## Acknowledgments

* Thanks to Splay Trees[https://www.geeksforgeeks.org/splay-tree-set-1-insert/] article on geeksForgeeks to understand the concepts related to it.
* Great thanks to our College professor for introducing us to the Data Structures subject and helping us learn the core concepts.
