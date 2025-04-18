# Challenge 01 - Browser Navigation System

## Overview

This is **Challenge 01** in the browser simulation series. The goal is to implement a basic browser navigation system that supports visiting new URLs, and navigating back and forward in history, similar to how real browsers function.

---

## Problem Statement

Design a `BrowserHistory` class that supports the following operations:

- `visit(url: str)` – Visit a new URL from the current page. Clears forward history.
- `back(steps: int)` – Move backward in history by `steps`. Return the current page.
- `forward(steps: int)` – Move forward in history by `steps`. Return the current page.

### Constraints

- All operations must run in **O(1)** time complexity.
- Use efficient data structures.
- Memory usage should be optimal for up to **10⁵** operations.

---

## Folder Structure

Each submission should reside in its own folder under the following structure:

/01-BrowserChallenges
|--01-BrowserNavigation
|-- solution.py
|-- README.md (Problem statement)
Copy the solution URL and submit in the provided Form.

---

## Submission Guidelines

1. Clone or fork the repository.
2. Create a folder named `01-BrowserNavigation` if it doesn't exist.
3. Write your solution in `solution.py`.
4. Use meaningful class/method names.
5. (Optional) Include comments or a `Solution.md` to explain your approach.
6. Ensure your code passes the provided test cases (or add your own).
7. Push your code and submit a PR for review.

---

## Suggested Starter Template

```python
class BrowserHistory:
    def __init__(self, homepage: str):
        pass

    def visit(self, url: str) -> None:
        pass

    def back(self, steps: int) -> str:
        pass

    def forward(self, steps: int) -> str:
        pass
```
