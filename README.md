# Experiment No. 7

## Title: Program Using React Hooks to Display Four Colour Buttons

## 1. Program Code

**File Name: src/App.jsx**

```jsx
import React, { useState } from "react";

function App() {

    // State to store selected color
    const [color, setColor] = useState("");

    return (

        <div
            style={{
                textAlign: "center",
                marginTop: "50px"
            }}
        >

            <h2>Select a Color</h2>

            {/* Buttons */}

            <button onClick={() => setColor("Red")}>
                Red
            </button>

            <button onClick={() => setColor("Blue")}>
                Blue
            </button>

            <button onClick={() => setColor("Green")}>
                Green
            </button>

            <button onClick={() => setColor("Yellow")}>
                Yellow
            </button>

            {/* Display Message */}

            {color && (
                <h3>You have selected: {color}</h3>
            )}

        </div>
    );
}

export default App;
```

## 2. Aim

To create a React application using the useState Hook that displays four colour buttons and shows the selected colour when a button is clicked.

## 3. Theory

- **React:** A JavaScript library used to build user interfaces.
- **Component:** A reusable part of a React application.
- **React Hooks:** Allow functional components to use state and other React features.
- **useState():** Stores and updates data in a component.
- **onClick:** Executes an action when a button is clicked.
- **setColor():** Updates the selected colour.
- **JSX:** Allows HTML-like elements to be written inside JavaScript.

## 4. Project Structure

A typical Vite + React project contains:

```text
color-selector/
│
├── node_modules/
├── public/
│
├── src/
│   ├── assets/
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── .gitignore
├── eslint.config.js
├── index.html
├── package.json
├── package-lock.json
├── README.md
└── vite.config.js
```

## 5. Steps to Execute

### Step 1: Create React Project

Open the VS Code terminal and enter:

```bash
npm create vite@latest color-selector -- --template react
```

### Step 2: Open Project Folder

```bash
cd color-selector
```

### Step 3: Install Dependencies

```bash
npm install
```

### Step 4: Add Program Code

Open the `src/App.jsx` file and replace its contents with the given React code.

### Step 5: Run the Application

```bash
npm run dev
```

### Step 6: Open in Browser

Open the local URL displayed in the terminal, usually:

```text
http://localhost:5173/
```

## 6. Output

The webpage initially displays:

```text
Select a Color

[Red]  [Blue]  [Green]  [Yellow]
```

### When Red Button Is Clicked

```text
You have selected: Red
```

### When Blue Button Is Clicked

```text
You have selected: Blue
```

### When Green Button Is Clicked

```text
You have selected: Green
```

### When Yellow Button Is Clicked

```text
You have selected: Yellow
```

## 7. Conclusion

Thus, the React program using the useState Hook was successfully implemented.

The application displays four colour buttons and dynamically shows the selected colour when a button is clicked.
