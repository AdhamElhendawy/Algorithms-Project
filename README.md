# Algorithms-Project
Longest Common Substring

Introduction
The Longest Common Substring problem involves finding the longest string (or strings) that is a substring (or are substrings) of two given strings. This is a classic problem in computer science and bioinformatics, often used in string matching and sequence alignment tasks.

Problem Statement
Given two strings, X of length m and Y of length n, find the length and the actual longest common substring of X and Y.

Dynamic Programming Approach
The dynamic programming approach to solve the Longest Common Substring problem is both efficient and easy to implement. The idea is to use a 2D table to store lengths of longest common suffixes of substrings. The longest common suffix is only considered if characters match.

Algorithm
Create a 2D array dp of size (m+1) x (n+1) to store lengths of longest common suffixes of substrings.
Initialize all values in dp to 0.
Iterate through each character of both strings. For each pair of characters:
If characters match, update the corresponding dp value to dp[i-1][j-1] + 1.
Track the maximum value in the dp table, which represents the length of the longest common substring.
Backtrack from the position of the maximum value in dp to get the longest common substring.

Complexity
Time Complexity: O(m * n), where m is the length of string X and n is the length of string Y.
Space Complexity: O(m * n), for the 2D array dp.

# project video #
https://www.youtube.com/watch?v=BzyOlUEdQKA
