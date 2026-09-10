# Linked List Implementation in JavaScript

## Overview
This project is a simple JavaScript implementation of a singly linked list. It includes the basic operations you would expect from a linked list, such as adding items, removing them, searching for values, and walking through the list.

The code is written with a small object-oriented structure and keeps the logic focused on the list itself rather than on any framework or external library.

## Features
- Append a value to the end of the list
- Prepend a value to the beginning of the list
- Get the current size of the list
- Access a node by its index
- Remove the last item
- Remove an item at a specific index
- Check whether a value exists in the list
- Find the index of a value
- Insert a value at a selected position
- Convert the list into a readable string form

## Installation
There are no external dependencies to install. You can use the file directly in a JavaScript project by importing the class:

```js
import { LinkedList } from './linked-list.js';
```

## Usage
### Create a linked list
```js
const list = new LinkedList();
```

### Add nodes
```js
list.append(10);
list.append(20);
list.prepend(5);
```

### Check the size
```js
console.log(list.size()); // 3
```

### Access a node by index
```js
console.log(list.at(1)); // node containing 10
```

### Remove nodes
```js
list.pop();
list.removeAt(0);
```

### Search for a value
```js
console.log(list.contains(10)); // true
console.log(list.contains(50)); // false
```

### Turn the list into a string
```js
console.log(list.toString()); // ( 10 ) -> null
```

## Edge cases covered
- Removing the final node correctly updates both the head and tail
- Removing from an empty list does nothing
- Accessing an index outside the list returns null
- Inserting past the end of the list is ignored
- Removing the only remaining node clears both head and tail

## Possible improvements
- Add a doubly linked list version
- Add a reverse method
- Support iteration with for...of

This project is a small, practical example of how a linked list can be built and used in JavaScript.

