# Objective-C Memory Management Bug

This repository demonstrates a common Objective-C memory management error involving an imbalance in `retain`/`release` calls, leading to memory leaks. The `bug.m` file contains the faulty code, while `bugSolution.m` provides the corrected version.

## Bug Description

The bug stems from the improper handling of memory ownership.  A retained object (`myString`) isn't properly released, causing a memory leak.  This type of error is particularly insidious as it may not manifest immediately, but rather gradually degrade application performance or cause unexpected crashes later on.

## Solution

The solution involves correctly balancing `retain` operations with `release` or `autorelease` calls. Using ARC (Automatic Reference Counting) is highly recommended to prevent such issues in modern Objective-C development.