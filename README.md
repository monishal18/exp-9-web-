# EXP 09 – React Lab Exercise: React Fragments

## NAME: Monisha L

## REG NO: 2305001019

---

## Aim

To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives

- Understand the concept of React Fragments.
- Use Fragment shorthand syntax.
- Use the explicit Fragment syntax.
- Group multiple JSX elements without an extra DOM node.
- Understand the difference between Fragments and div elements.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: App.jsx – Using Fragment Shorthand

```jsx
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name: Monisha</h3>

      <p>Register Number: 2305001019</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
```

### Step 3: Using Explicit Fragment Syntax

```jsx
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>

      <p>Name: Monisha</p>

      <p>Register Number: 2305001019</p>

      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>

      <Student />
    </Fragment>
  );
}

export default App;
```

## Output

### 1. Fragment Shorthand Syntax

<img width="597" height="330" alt="image" src="https://github.com/user-attachments/assets/a8209b10-bbf6-42fe-a96e-948a577012ef" />



### 2. Explicit Fragment Syntax

<img width="557" height="271" alt="image" src="https://github.com/user-attachments/assets/16dfd453-58f6-4457-a49d-75e58f80d6b0" />


## Result

Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.
