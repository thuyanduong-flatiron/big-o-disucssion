# big-o-disucssion


They say that there are multiple ways to skin a cat. Concurrently, there are also multiple ways for developers to come up with an algorithm to solve a problem. A simple example would be sorting items in an array. You can use bubble sort, merge sort, quick sort, etc., to solve this particular problem.

But how do we know which algorithm is the best one? It would be nice to have a rating scale that would let us point to the best solution. Unfortunately, we don’t have that yet! Instead, computer scientists have come up with a way to calculate the efficiency of algorithms commonly known as Big O.

## Big O Notation

Big O notation is a mathematical notation that describes a function as the value of the input increases. Basically, Big O is the language and metric we use to describe the efficiency of algorithms. When analyzing an algorithm, we look at the Time complexity and Space complexity. Some of the most common runtimes are O(1), O(log N), O(N log N), O(N), O(N²), and O(2ⁿ). There’s no fixed list of possible runtimes.

Note: When calculating Big O, we always assume the worst-case scenarios for each algorithm.

> “Time complexity of an algorithm quantifies the amount of time taken by an algorithm to run as a function of the length of the input. Similarly, Space complexity of an algorithm quantifies the amount of space or memory taken by an algorithm to run as a function of the length of the input increases.” —HackerEarth
Why Use Big O?

Since Big O assumes the worst-case scenario, we’re guaranteed that our program will finish within a time period. It may or may not stop earlier but never later. The most commonly known use case of optimization of an algorithm is Google’s search engine. Currently, there are 1.8 billion websites available on the internet. That’s a lot of data! Therefore, Google has to optimize their algorithms in order to serve you those massive amounts of data in the shortest time possible. This is where Big O comes into play.

## Introduction and Reference Guide

My focus in this piece is to help you understand the tricky bits of Big O notation by analyzing the Big O of simple JavaScript functions that could possibly be asked in an interview. If this is your first time encountering Big O notation, then I highly suggest you take a look at this in-depth YouTube video explanation on complexities before attempting any of these questions. This article assumes basic knowledge of data structures and loops.

Before we go ahead and solve the questions, let’s refresh our memory by using this reference guide.

* Drop the constants - Big O notation doesn't care about constants because Big O notation only describes the long-term growth rate of functions. So drop the constants, no matter how large they are.
* Drop the non-dominant terms - Using Big O notation, we're interested in the upper bound.Therefore non-dominant terms are non-important.
* Add vs. multiply - We add when there is a separate chunk of work(separate for-loops) in a function, and we multiply when we combine chunks of work(nested for-loops).
* Log N runtimes - We use Log N if the array range gets divided into half of the current range in a for-loop.Constant time algorithms are the quickest. Logarithmic time(log N) is the second quickest.Mostly used in binary search.
* Recursive runtimes - Runtimes of a recursive function with multiple branches is typically O( branchesᵈᵉᵖᵗʰ ).
* Derive by counting iteration - Do not memorize common patterns; rather, deeply comprehend the algorithms and monitor the iterations, for they will give you a hint in deriving the time complexity.










[Reference to original blog post](https://medium.com/better-programming/cracking-the-big-o-notation-interview-questions-4ec56f14b026) 
