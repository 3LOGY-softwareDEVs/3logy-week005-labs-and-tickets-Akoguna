# LAB 19: Timer & Data Fetcher

**Week:** 5 — Wednesday  
**Points:** 12.5  
**Due:** Wednesday EOD

---

## 🎯 OBJECTIVE

Build two mini-applications that demonstrate key useEffect patterns: a **Stopwatch/Timer** and a **Data Fetcher** component.

---

## 📋 REQUIREMENTS

### Part 1: Stopwatch Timer
- [ ] Start/pause/reset functionality
- [ ] Displays minutes and seconds (MM:SS format)
- [ ] Uses `useEffect` with `setInterval`
- [ ] Proper cleanup function (clears interval)
- [ ] Lap recording (bonus)

### Part 2: Data Fetcher
- [ ] Fetches data from `https://jsonplaceholder.typicode.com/posts`
- [ ] Shows loading state while fetching
- [ ] Shows error state if fetch fails
- [ ] Displays list of posts (title + body preview)
- [ ] Uses `useEffect` with empty dependency array `[]`
- [ ] Search/filter posts by title (uses state + filtered rendering)

### Technical Requirements:
- [ ] At least 2 `useEffect` calls (one for timer, one for fetch)
- [ ] Proper dependency arrays
- [ ] Cleanup function for timer
- [ ] Loading and error states for data fetching
- [ ] No console errors or warnings

---

## 💡 STARTER CODE

```jsx
import React, { useState, useEffect } from 'react';

function App() {
  return (
    <div>
      <h1>useEffect Patterns</h1>
      <StopWatch />
      <hr />
      <PostList />
    </div>
  );
}

function StopWatch() {
  const [seconds, setSeconds] = useState(0);
  const [isRunning, setIsRunning] = useState(false);

  // TODO: useEffect with setInterval
  // TODO: cleanup function

  return (
    <div>
      <h2>⏱️ Stopwatch</h2>
      {/* TODO: Display time, start/pause/reset buttons */}
    </div>
  );
}

function PostList() {
  const [posts, setPosts] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);
  const [search, setSearch] = useState('');

  // TODO: useEffect to fetch posts

  return (
    <div>
      <h2>📄 Posts</h2>
      {/* TODO: Search input, loading state, error state, post list */}
    </div>
  );
}

export default App;
```

---

## ✅ ACCEPTANCE CRITERIA

- [ ] Stopwatch counts up correctly
- [ ] Start/pause/reset all work
- [ ] Timer cleans up on component changes
- [ ] Posts load from API successfully
- [ ] Loading spinner/message shown while fetching
- [ ] Error handled gracefully
- [ ] Search filters posts in real-time

---

## 📤 SUBMISSION

```
LAB-19 Submission
Name: [Your Name]
GitHub: [Repository URL]
Features: ✅ Timer ✅ Cleanup ✅ Fetch ✅ Loading ✅ Search
```
