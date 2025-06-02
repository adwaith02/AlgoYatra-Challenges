
---

## 📘 Challenge 02 - Browser Tab Management

Welcome to **Challenge 02** of the **AlgoYatra Browser Series**!

In this challenge, you're tasked with implementing **tab management** functionality for a minimal browser simulation. This is a continuation of Challenge 01 (Browser Navigation), where we built the basic back/forward navigation system.

This time, we'll focus on handling **multiple tabs**, switching between them, closing them, and ensuring that each tab retains its own navigation state independently.

---

### 🔧 Features to Implement

You need to build a class `Browser` with the following features:

#### 🗂 Tab Operations

* `new_tab(url: str) -> int`:
  Open a new tab with a given `url` as its homepage. Returns a unique `tab_id`.

* `switch_tab(tab_id: int) -> bool`:
  Switch to the tab with the given ID. Returns `True` if successful, else `False`.

* `close_tab(tab_id: int) -> bool`:
  Closes the specified tab. If the closed tab is the currently active tab, switch to another open tab (any one of them). If no tabs are left, set the active tab to `None`.

#### 🌐 Navigation Within Tabs

Each tab must retain its own independent:

* `visit(url: str)`
* `back(steps: int)`
* `forward(steps: int)`
* `current_url() -> str`

These should behave exactly like they did in **Challenge 01**.

---

### 📂 Folder Structure & Submission Guide

Your repo should follow this structure for submission:

```
/02-BrowserChallenges/
  └── 02-TabManagement/
        ├── browser.py           # Your implementation
        └── test_browser.py      # Unit tests (provided or created by you)
```

---

### ✅ Functional Expectations

* Each tab maintains **independent** history state.
* Switching between tabs does not corrupt history.
* Closing a tab and switching between remaining tabs should work gracefully.

---

### 💻 Sample Run (Conceptual)

```python
b = Browser()
tab1 = b.new_tab("leetcode.com")
tab2 = b.new_tab("github.com")

b.switch_tab(tab1)
b.visit("google.com")
b.back(1)  # back to leetcode.com

b.switch_tab(tab2)
b.visit("openai.com")
b.back(1)  # back to github.com

b.switch_tab(tab1)
print(b.current_url())  # Should still be leetcode.com
```

---

### 🧪 How to Run Tests

Make sure you are inside the `02-TabManagement` directory.

```bash
python3 -m unittest -v test_browser.py
```

You should see a detailed breakdown of all test cases and print logs showing the test progress.

---

### 📤 Submission Instructions

Once completed:

1. Push your code to your **own GitHub repo**.
2. Structure your submission inside the folder:

   ```
   02-BrowserChallenges/02-TabManagement/
   ```
3. Submit the **link to your GitHub repo** using the form (we will provide the link here).

---

### ⏱ Suggested Time

**60–90 minutes** (including writing test cases).

---

### 🧠 Bonus Ideas (Optional)

Try extending this challenge by adding:

* `list_tabs()` to show all open tabs.
* `reopen_closed_tab()` with history restoration.
* Tab titles or favicons.

---

Happy Building 🚀
*The AlgoYatra Team*

---
