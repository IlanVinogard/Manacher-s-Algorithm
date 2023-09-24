# Manacher-s-Algorithm

## Programming Language

This project is developed using the C++ programming language. All the source code and examples are written in C++.

## Used Algorithm

In this project, the Manacher's Algorithm was used for finding palindromes within a string. The implementation of this algorithm was provided by [elfarouk-etawilv](https://leetcode.com/elfarouk-etawilv/) on LeetCode. You can find the original code and its author [here](https://leetcode.com/elfarouk-etawilv/).

## Manacher's Algorithm

Manacher's Algorithm is an efficient algorithm used for finding the longest palindromic substring within a given string. It achieves a time complexity of O(n), making it significantly faster than the brute force approach, which has a time complexity of O(n^3).

The algorithm works by creating a new string from the input string and adding special characters, such as '$' and '#', to enable the detection of palindromes with both odd and even lengths. For example, if the input string is "aba," the new string becomes "$#a#b#a#."

Manacher's Algorithm maintains an array of the same length as the new string to keep track of the palindrome sizes. It then iterates through the new string, checking if it can expand a palindrome at each position. If it can expand, it increments the corresponding element in the array to denote the size of the current palindrome. If not, it continues to the next position.

The algorithm also keeps track of the rightmost palindrome boundary and its center. If a new palindrome extends beyond the rightmost boundary, it updates these values accordingly.

Finally, the algorithm returns the longest palindromic substring using the `substr` function.

## License

This project is licensed under the [license name, e.g., MIT License]. Please refer to the LICENSE file for details.
