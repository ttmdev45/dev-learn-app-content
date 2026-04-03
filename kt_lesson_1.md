# Sealed Classes & Pattern Matching (Kotlin)

## Introduction

In Kotlin, **sealed classes** and **pattern matching (`when`)** are powerful tools used to:

- represent restricted class hierarchies
- model UI states and API responses
- write safer and more predictable code

They are widely used in **Android development**, especially with **Jetpack Compose** and **MVVM architecture**.

---

# What is a Sealed Class?

## Definition

A **sealed class** is a special type of class that restricts which classes can inherit from it.

👉 All subclasses must be defined in the **same file**

---

## Why Use Sealed Classes?

- safer than `open` classes
- better than `enum` for complex data
- ensures all cases are handled
- works perfectly with `when`

---

## Basic Syntax

```kotlin
sealed class Result {
    object Loading : Result()
    data class Success(val data: String) : Result()
    data class Error(val message: String) : Result()
}
