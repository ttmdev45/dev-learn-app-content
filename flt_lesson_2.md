# Mastering Collection If & Collection For

## Introduction

In Flutter, `Collection if` and `Collection for` are very useful features in Dart.  
They help us build widget lists more cleanly, dynamically, and with less repeated code.

These features are commonly used inside:

- `children: []`
- `items: []`
- any `List<Widget>`
- any Dart collection like `List`, `Map`, and `Set`

Using them makes Flutter UI code easier to read and maintain.

---

## What is Collection If?

`Collection if` allows you to add an item into a collection only when a condition is true.

### Syntax

```dart
[
  if (condition) item
]