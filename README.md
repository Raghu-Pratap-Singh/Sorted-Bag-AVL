# Sorted Bag (AVL Tree Implementation)

[![PyPI version](https://img.shields.io/pypi/v/sorted-bag-avl.svg)](https://pypi.org/project/sorted-bag-avl/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A high-performance, self-balancing **Sorted Bag** (multiset) implemented using an **AVL Tree**. This package provides $O(\log n)$ efficiency for insertions, deletions, and lookups, while maintaining elements in sorted order.

## Features
- **Self-Balancing**: Uses AVL tree logic to ensure the tree height is always logarithmic.
- **Fast Indexing**: Support for finding the $k$-th smallest element in $O(\log n)$ time.
- **Range Queries**: Efficiently count or retrieve elements within a specific range.
- **Duplicate Support**: Handles multiple instances of the same value.

## Installation

Install the package via pip:

```bash
pip install sorted-bag-avl
