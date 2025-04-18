# 🧪 Test Case Scenarios - Browser Navigation System

Use the following scenarios to test your implementation of the `BrowserHistory` system. These are language-agnostic and described step by step.

---

## Test Case 1

1. Initialize with homepage: `"home.com"`
2. Visit `"search.com"`
3. Visit `"news.com"`
4. Visit `"videos.com"`
5. Go back by 1 step → should return `"news.com"`
6. Go back by 1 step → should return `"search.com"`
7. Go forward by 1 step → should return `"news.com"`
8. Visit `"profile.com"` (forward history should be cleared)
9. Go forward by 2 steps → should return `"profile.com"`
10. Go back by 2 steps → should return `"search.com"`
11. Go back by 5 steps → should return `"home.com"`

---

## Test Case 2

1. Initialize with homepage: `"index.com"`
2. Visit `"blog.com"`
3. Visit `"forum.com"`
4. Go back by 1 step → should return `"blog.com"`
5. Go back by 1 step → should return `"index.com"`
6. Go forward by 1 step → should return `"blog.com"`
7. Visit `"support.com"` (forward history should be cleared)
8. Go forward by 2 steps → should return `"support.com"`
9. Go back by 1 step → should return `"blog.com"`

---

## Edge Case - Large Navigation Steps

1. Initialize with homepage: `"startpage.com"`
2. Visit pages `"site1.com"` through `"site99.com"` (99 visits total, i.e., `site1.com`, `site2.com`, ..., `site99.com`)
3. Go back by 150 steps → should return `"startpage.com"`
4. Go forward by 150 steps → should return `"site99.com"`

---

Feel free to expand on these scenarios to stress test your solution under different conditions.
