# LAB 18: Interactive Todo App

**Week:** 5 — Tuesday  
**Points:** 12.5  
**Time:** 45 minutes (in class) + homework  
**Due:** Tuesday EOD

---

## 🎯 OBJECTIVE

Build a fully functional **Todo Application** using React state management (useState). Practice adding, toggling, deleting, and filtering items in state.

---

## 📋 REQUIREMENTS

### Core Features:
- [ ] Add new todos via text input + button
- [ ] Mark todos as complete (checkbox toggle)
- [ ] Delete individual todos
- [ ] Filter todos: All / Active / Completed
- [ ] Display count of remaining active todos
- [ ] Clear all completed todos button

### Technical Requirements:
- [ ] useState for todos array, input value, and filter
- [ ] Immutable state updates (spread, map, filter)
- [ ] Unique `key` prop on all list items (use Date.now() for IDs)
- [ ] Controlled input (value + onChange)
- [ ] Enter key support for adding todos
- [ ] No console errors

---

## 💡 STARTER CODE

```jsx
import React, { useState } from 'react';
import './App.css';

function App() {
  const [todos, setTodos] = useState([]);
  const [inputValue, setInputValue] = useState('');
  const [filter, setFilter] = useState('all');

  // TODO: addTodo function
  // TODO: toggleTodo function  
  // TODO: deleteTodo function
  // TODO: clearCompleted function
  // TODO: getFilteredTodos function

  const activeCount = todos.filter(t => !t.completed).length;

  return (
    <div className="App">
      <h1>📝 React Todo List</h1>
      {/* TODO: Input section */}
      {/* TODO: Filter buttons */}
      {/* TODO: Todo list */}
      {/* TODO: Footer with count and clear button */}
    </div>
  );
}

export default App;
```

---

## ✅ ACCEPTANCE CRITERIA

- [ ] Can add todos (button click and Enter key)
- [ ] Can toggle todos complete/incomplete
- [ ] Can delete individual todos
- [ ] Filter buttons work (All, Active, Completed)
- [ ] Active count updates correctly
- [ ] Clear completed removes all done todos
- [ ] Empty state message when no todos
- [ ] Clean, well-organized code

---

## 🏆 BONUS

- [ ] Edit todo text (double-click to edit)
- [ ] Persist todos to localStorage
- [ ] Add due dates to todos
- [ ] Drag to reorder
- [ ] CSS animations for add/remove

---

## 📤 SUBMISSION

```
LAB-18 Submission
Name: [Your Name]
GitHub: [Repository URL]
Screenshot: [Show todos with different states]
Features: ✅ Add ✅ Toggle ✅ Delete ✅ Filter ✅ Count
```
