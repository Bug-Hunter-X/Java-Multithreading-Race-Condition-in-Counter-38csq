# Java Multithreading Race Condition

This repository demonstrates a common race condition that can occur in multithreaded Java programs.  The `Counter` class is designed to increment a counter, but without proper synchronization, multiple threads accessing it concurrently can lead to incorrect results.

The `Main` class creates two threads that increment the counter 10,000 times each.  The expected final count is 20,000, but due to the race condition, the actual count is often less.

The solution demonstrates how to fix the race condition using the `synchronized` keyword.