Matrix Layer Rotation
Problem Statement

Given an m × n matrix and a rotation count r, rotate each layer (ring) of the matrix in an anti-clockwise direction by r positions and print the resulting matrix.

Approach
Divide the matrix into concentric layers.
Extract elements of each layer into a temporary list.
Rotate the list anti-clockwise using r % layerLength.
Insert the rotated elements back into their respective layer positions.
Print the final rotated matrix.
Features
Efficiently handles large rotation counts.
Rotates each matrix layer independently.
Works for rectangular as well as square matrices.
Compatible with Java 7.
Algorithm
Identify the number of layers: min(m, n) / 2.
For each layer:
Extract boundary elements.
Rotate the extracted list.
Refill the layer with rotated values.
Output the transformed matrix.
Time Complexity
O(m × n)
Space Complexity
O(m × n)
Technologies Used
Java 7
ArrayList
List Interface
BufferedReader for input handling
Sample Input
4 4 2
1 2 3 4
5 6 7 8
9 10 11 12
13 14 15 16
Sample Output
3 4 8 12
2 11 10 16
1 7 6 15
5 9 13 14
