# Indexing for High Performance

Index are used to find rows quickly. Index optimization is perhaps the most powerful way to improve query performance.

## Indexing basics

In MySQL, a storage engine searches the index's data structure for a value. When it finds a match, it can find the row that contains the match.

### B-Tree indexes

Use a B-Tree data structure to store data. (Many storage engines actually use a B+Tree index, in which each leaf node contains a link to the next for fast range traversals through nodes.)

The general idea of a B-Tree is that all the values are stored in order, and each leaf page is the same distance from the root.
