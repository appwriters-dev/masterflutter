---
id: ls01-introduction-to-asynchronous-programming
title: Introduction to Asynchronous Programming
description: Asynchronous programming is a programming paradigm that enables a program to do more than one thing at a time. In asynchronous programming, long-running tasks run in the background without blocking the main execution thread. Asynchronous programming is very useful for performing I/O operations, such as accessing the network and accessing the file system. Dart uses Future, Stream, and async/await to implement asynchronous programming.
---

Asynchronous programming is a programming paradigm that allows a program to do multiple things at the same time. Long-running tasks in asynchronous programming run in the background without interfering with the main execution thread. Asynchronous programming is extremely useful for performing I/O operations such as network and file system access. Asynchronous programming can also be used to perform time-consuming tasks like image processing and mathematical calculations.

Asynchronous programming is used in Dart and Flutter for a variety of tasks, including:

- Using HTTP to make REST API requests
- Reading and writing files 
- Completing complex calculations
- Executing lengthy tasks, such as animations

In this chapter, we will learn about asynchronous programming in Dart and Flutter. We will learn about the `Future` class, the `async` and `await` keywords, and the `Stream` class.

## Projects

### 1. Every 5 Second

Write a program that prints current time after 5 seconds.

### 2. Read a File

Write a Program that reads a text file and prints the contents of the file to the console

### 3. Multiple Futures

Write a program that uses the Future class to perform multiple asynchronous operations in parallel, and then uses the Future.wait() method to wait for all the operations to complete before continuing.

## Resources

- [DartPad: Futures](https://dartpad.dev/futures)
- [Dart Async and Await](https://dart.dev/codelabs/async-await)
- [Asynchronous Programming](https://dart-tutorial.com/asynchronous-programming/asynchronous-programming-in-dart/)
- [Future in Dart](https://dart-tutorial.com/asynchronous-programming/future-in-dart/)
- [Async and Await in Dart](https://dart-tutorial.com/asynchronous-programming/async-and-await-in-dart/)
