#dart #coursera 

Mobile, desktop, web and server

Foundation of flutter framework

Runs on a VM, compiled, quick and efficient

Checked and optimized at compile time

Uses Just-in-time(JIT) and Ahead-of-time(AOD) compilation

## JIT
- Happens while program is running
- Shows changes without having to restart app
- Good for development

## AOT
- Happens before running program
- Apps starts faster and runs smoother
- Better for release

## Garbage Collection

Generational garbage collection strategy 

Divides up objects by generation by age

### Young Generation

Young generation are temp or needed for short time 

Cleaned up frequently

eg: Messages

### Old Generation

Used more often and for longer periods

Cleaned less often as the will likely be used again

eg: Contacts

## Concurrency

Handled with Isolates and async programming

eg: Waiting for data from internet to load. App is interactable while data is loading

Another eg: loading from a file


### Isolates

Run at the same time and don't share memory

This prevents problems caused by different things sharing memory

They communicate by sending messages to each other

### Async

Uses `async` and `await` keywords

Create code that runs while waiting for something else to finish

## Core Libraries

### dart:core

`dart:core` is included in every Dart program

Provides basic functions and classes like numbers, strings, and lists

### dart:async 

Helps with a sync programming

Includes classes like `Future` and `Stream` to handle tasks that take time to complete

### dart:io 

Handles input and output, reading and writing files, and connecting to the internet

### dart:convert

Helps convert data 

eg: JSON to Dart objects and vice versa

### dart:math

Provides mathematical functions and constants useful for complex operations

