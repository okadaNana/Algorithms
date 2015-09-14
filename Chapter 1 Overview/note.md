# Chapter 1: Overview
## Question
* What are data structures and algorithms?
* What good will it do me to know about them?
* Why can't I just use arrays and *for* loops to handle my data?
* When does it make sense to apply what I learn here?

## What Are Data Structures and Algorithms Good For?
**Data Structures**

> A *data structures* is an arrangement of data in a computer's memory (or sometimes on a disk).

Data structures include arrays, liked lists, stacks binary trees, and hash tables, among others.

**Algorithms**

> *Algorithms* manipulate the data in these structures in various ways, such as searching for a particular data item and sorting the data.

What sorts of problems can you solve with a knowledge of these topics?
* Real-world data storage
* Programmer's tools
* Modeling

**Real-World Data Storage**
Suppose you want to update you old index-card system to a computer program. You might find yourself with questions like these:
* How would you store these data in your computer's memory?
* Would your method work for a hundred file cards? A thousand? A million?
* Would your method permit quick insertion of new cards and deletion of old ones?
* Would it allow for fast searching for a specified card?
* Suppose you wanted to arrange the cards in alphabetical order. How would you sort them?

**Programmer's Tools**
Real-Wold data is accessed more or less directly by program's user. Some data storage structures, however, are not mean to accessed by the user, but by the program itself. Stacks, queues, and priority queues are often used in this way.

**Real-World Modeling**
The most import data structure of this type is graph. You can use graphs to represent airline routs between cities or connections in an electric circuit or tasks in a project.

A queue, can model customers waiting in line at a bank or cars waiting at a toll booth.

## Overview of Data Structures
**Characteristics of Data Structures**
|Data Structures    |Advantages         |Disadvantage       |
|:------------------|:------------------|:------------------|
|Array|Quick insertion, very fast access if index known.|Slow search, slow deletion, fixed size.|
|Order array|Quicker search than unsorted array|Slow insertion and deletion, fixed size|
|Stack|Provides last-in, first-out acceess.|Slow access to other items.|
|Queue|Provide first-in, first-out access.|Slow access to other items.|
|Linked list|Quick insertion, quick deletion|Slow search.|
|Binary tree|Quick search, insertion, deletion (if tree remains balanced).|Deletion algorithm is complex.|
|Red-black tree|Quick search, insertion, deletion. Tree always balanced.|Complex.|
|2-3-4 tree|Quick search, insertion, deletion. Tree always balanced. Similar trees good for disk storage.|Complex.|
|Hash table|very fast access if key known. Fast insertion.|Slow deletion, access slow if key not know, inefficient memory usage.|
|Heap|Fast insertion, deletion, access to largest item.|Slow access to other items.|
|Graph|Models real-world situations.|Some algorithms are slow and complex.|

## Overview of algorithms
* Insert a new data item.
* Search for a specified  item.
* Delete a specified item.
* *Iterate*  through all the items in a data structures.
* *Sorting* data.