# Sorted Bag (AVL Tree Implementation)

[![PyPI version](https://img.shields.io/pypi/v/sorted-bag-avl.svg)](https://pypi.org/project/sorted-bag-avl/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A high-performance, self-balancing **Sorted Bag** (multiset) implemented using an **AVL Tree**. This package provides $O(\log (u)$ efficiency for insertions, deletions, and lookups, and order statistics while maintaining elements in sorted order.

## Features
- **Self-Balancing**: Uses AVL tree logic to ensure the tree height is always logarithmic.
- **Fast Indexing**: Support for finding the $k$-th smallest element in $O(\log (u))$ time.
- **Range Queries**: Efficiently count or retrieve elements within a specific range.
- **Duplicate Support**: Handles multiple instances of the same value.


## FUNCTIONS AVAILABLE

- **Standard Python Functions**: print, max, min, indexing, membership check(x in S).
- **Order Statistics (O(log (u)))**: S.kth(rank), S.lower_bound(x), S.upper_bound(x), S.lesser_than(x), S.greater_than(x), S.range_count(x), S.count(x).

## Technical Explanation: $O(\log u)$ Complexity
Unlike standard implementations where the tree height is determined by the total number of elements ($n$), this package uses a **Frequency-Augmented AVL Tree**. 

Each node stores a `count` for duplicate values. Therefore, the tree height is proportional only to the number of **unique** elements ($u$). This ensures that even with millions of duplicate entries, the search path remains extremely short, providing a significant performance boost over standard $O(\log n)$ structures.


## Installation

Install the package via pip:

```bash
pip install sorted-bag-avl

