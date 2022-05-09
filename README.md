# Mos-Algorithm

## Overview
Python implementation of Mo's Algorithm - a method for answering a series of
range queries on the same array.

Running time and space complexity of this method are:
<p align=center>
<img src="https://github.com/jyuv/Mos-Algorithm/blob/main/assets/mos_times.png?raw=true">
</p>
 
 The repository provides a general interface for Mos operations to later
 be adjusted to specific tasks, and 2 examples of such tasks.
 
 ### Use Case Example 1 - Sum In Range
Given an array this example answers efficiently a series of range queries
where each query calculate the sum of its range.
  ```python
from mos_algorithm import MosAlgorithm, SumInRange
input_array = [1, 1, 2, 1, 3, 4, 5, 2, 8]
queries = [(0, 4), (1, 3), (2, 4)]
case1 = MosAlgorithm(input_array, queries)
case1.run_queries(SumInRange)
````
 
 ### Use Case Example 2 - Unique Items In Range
Given an array this example answers efficiently a series of range queries
where each query calculate the number of unique items in its range.
 ```python
from mos_algorithm import MosAlgorithm, UniqueItemsInRange
input_array = [1, 1, 2, 1, 3, 4, 5, 2, 8]
queries = [(0, 4), (1, 3), (2, 4)]
case1 = MosAlgorithm(input_array, queries)
case1.run_queries(UniqueItemsInRange)
````