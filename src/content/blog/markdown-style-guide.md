---
title: Let's become a super hero in data structures!
description: Here is a sample of some basic Markdown syntax that can be used
  when writing Markdown content in Astro.
pubDate: Apr 25 2023
publishDate: 2023-04-25T16:16:46.096Z
heroImage: /placeholder-hero.jpg
---
If you're one of those geeks interested in coding interviews and jobs in big tech companies, you probably have heard about data structures before. Data structures are often implemented using classes or primitives in programming languages to organize and store data efficiently. They are fundamental concepts in computer science and are essential for solving complex problems efficiently. In this blog post, we will explore some of the most important data structures, their use cases, and how they can be implemented. Whether you're a beginner or an experienced developer, this post will provide you with a solid foundation to understand data structures and their role in computer science. So, let's dive in!
So first let's list all the data structures we're going to discuss in this post:
- Arrays
- Linked Lists (Including doubly linked lists).
- Queue
- Stack
- Trees
- Graphs (Only basic stuff).
- Hash Tables.
- Heaps.
# 1. Arrays
In computer science, an array is a linear data structure that stores a collection of values, those values are typically of the same data type. In programming languages like `C#`, `C++`, `Java` or other programming languages arrays have a fixed size that is given to the compiler at compilation time, this size cannot be modified during Run-Time. Similarly, the data type of the values that the array can store is fixed at compilation and cannot be modified later. Arrays give us the ability to iterate over elements in a linear manner and access any values at any given index in an efficient way, the time at which we can access a value by its index is constant.
 Let's take a look at a very basic problem which can be used using arrays:
> Write a program that receives **10 integers** from the user. In the end, the program should print all ten numbers and their average.
So first, how do we know we need to use an array here? The critical part here is the part we're asked to print all ten numbers after all of them have been received. If we dropped this part we could do something similar to this:
1. Define a variable called `sum`
2. Increment the value of `sum` by each number received.
3. Print `sum/10` to the screen.
We've been asked to print all ten numbers though, how could we make the program remember all numbers? Well, we'll need something that can store all those numbers so we can come back to them in the end and print each one of them to the screen.
The most basic thing that gives all those features with good efficiency is an array. The solution to the problem could be as follows:
1. Declare an array that will hold 10 integers, and an integer variable that will hold the sum of the numbers.
2. Use a `for` loop to do `10` iterations.
3. Read an integer from the user in each iteration.
4. Append the number to the array.
5. Add it to the `sum` variable.
6. Loop over all numbers and print them and then print the value of `sum/10`.
> Notice: The `sum` variable didn't really save us a lot in this problem. we had to loop over all numbers in the end either way, that's because we have to print them one by one, so we could sum them up in the same loop that prints them.