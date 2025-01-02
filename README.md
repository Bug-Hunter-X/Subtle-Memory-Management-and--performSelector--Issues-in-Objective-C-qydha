# Objective-C: Subtle Memory Management and `performSelector` Pitfalls

This repository demonstrates two common yet easily overlooked issues in Objective-C programming: improper memory management and the potential dangers of using `performSelector` without adequate precautions. The `bug.m` file contains code exhibiting these problems.  `bugSolution.m` provides corrected versions with explanations of the fixes.

## Memory Management

Objective-C's manual memory management (or even ARC's automated management) can be tricky. Failure to manage object lifecycles properly often leads to memory leaks or crashes.  The example illustrates how this can happen if not handled carefully. 

## `performSelector` Issues

The use of `performSelector` offers flexibility, but it also introduces potential runtime issues such as `selector` not found exceptions. These exceptions are difficult to debug if not handled proactively.

## Solutions

The `bugSolution.m` file presents the corrected implementations, emphasizing best practices for memory management and the safer usage of `performSelector` (or better alternatives). It demonstrates how to prevent memory leaks and handle potential exceptions gracefully.