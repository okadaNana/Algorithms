# Arrays

## Questions
* The Basics of Arrays in Java
* Dividing a Program into Classes
* Class Interfaces
* Java Code for an Ordered Array
* Logarithms
* Big O Notation
* Why Not Use Arrays for Everything?

The arrays is the most commonly used data storage structure. They offer a convenient jumping-off place for introducing data structures.

These three operations - insertion, searching, and deletion - will be the fundamental ones in most of the data storage structures we'll study in this book.

## Duplicates OK Versus No Duplicates
|operation|No Duplicates|Duplicates OK|
|:---:|:---:|:---:|
|Search|N/2 comparisons|N comparisons|
|Insertion|No comparisons, one move|No comparisons, one move|
|Deletion|N/2 comparisons, N/2 moves|N comparisons, move than N/2 moves|

## Class Interfaces
If a class is used by many different programmers, the class should be designed so that it's easy to use. That way that a class user relates to the class is called the class *interface*.

## Abstraction
OOP is distribute what and how.

The process of separating the *how* from the *what* - how an operation is performed inside a class, as opposed to what's visible to the class user - is call abstraction.

Abstraction is an important aspect of software engineering. By abstracting class functionality, we make it easier to design a program because we don't need to think about implementation details at too early a stage in the design process.

## Binary Search
```java
public int find(long searchKey) {
	int lowerBound = 0;
	int upperBound = nElems - 1;
	int curIn;

	while (true) {
		curIn = (lowerBound + upperBound) / 2;
		if (a[curIn] == searchKey) {
			return curIn;     // found it
		} else if (lowerBound > upperBound) {
			return nElems;	  // can't find it
		} else {              // divide range
			if (a[curIn] > searchKey) {
				lowerBound = curIn + 1;  // it's in upper half
			} else {
				upperBound = curIn - 1;  // it's in lower half
			}
		}
	}
}
```

## Advantages and Disadvantage of Order Arrays
The major advantage is that search times much faster than in unordered array.

The disadvantage is that insertion takes longer because all the data item with a higher key value must be moved up to make room.

Deletion are slow in both ordered and unordered arrays because items must be moved down to fill the hole by the deleted item.

Ordered arrays are therefore useful in situation in which searches are frequent, but insertion and deletion are not.