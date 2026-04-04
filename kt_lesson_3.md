## Expect / Actual Pattern Guide (Kotlin Multiplatform)

## Introduction

The **Expect/Actual pattern** is a core concept in **Kotlin Multiplatform (KMP)**.

It allows you to:

- write shared (common) code
- provide platform-specific implementations
- keep your business logic reusable across platforms (Android, iOS, Web, etc.)

---

## Why Use Expect / Actual?

In multiplatform projects, some features depend on the platform:

- file system access
- network APIs
- device hardware
- secure storage
- logging

👉 You cannot implement these once in common code.

So Kotlin provides:

- `expect` → declaration in shared code
- `actual` → implementation in platform code

---

## 1. How It Works

## Concept

| Layer | Role |
|------|------|
| commonMain | declare expected API |
| androidMain / iosMain | provide actual implementation |

---

## Flow

```text
commonMain (expect) → androidMain / iosMain (actual)