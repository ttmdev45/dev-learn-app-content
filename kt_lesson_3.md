# Generics & Variance (In/Out) (Kotlin)

## Introduction

Generics in Kotlin allow you to write **flexible and reusable code** by working with different data types safely.

Variance (`in` / `out`) helps control how generic types behave in inheritance.

👉 Together, they provide **type safety + flexibility**

---

# 1. What are Generics?

## Definition

Generics allow classes and functions to operate on **different types** while maintaining type safety.

---

## Example (Without Generics ❌)

```kotlin
class Box(val value: Any)