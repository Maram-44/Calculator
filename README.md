# 🧮 Custom UI & Polish Notation Calculator

A high-performance Desktop Calculator application built using **C# and Windows Forms (WinForms)**. This project serves as a deep dive into two core software engineering domains: creating fully reusable **Custom UI Controls** from scratch, and implementing an advanced mathematical parser based on **Prefix/Postfix (Polish Notation)** algorithms.

---

## 🚀 Key Project Focus Areas

### 1. Reusable Custom UI Controls
Instead of relying on standard, generic Windows Forms buttons and displays, this project implements customized components:
*   **Custom Calculator Buttons:** Inheriting from the base control class with overridden drawing states (Hover, Click, Focus) to achieve a modern, sleek visual layout.
*   **Encapsulated Logic:** Every custom button securely holds and passes its own state and mathematical operators without cluttering the main Form's event pipeline.

### 2. Prefix / Postfix Expression Evaluation (Polish Notation)
Standard string evaluation can easily break down with complex operational hierarchies. This app solves that by parsing inputs into an optimized notation stack:
*   **Operator Precedence Mastery:** Dynamically converts user input into a logical evaluation tree/stack, ensuring operations like Multiplication (`*`) and Division (`/`) execute with absolute priority over Addition (`+`) and Subtraction (`-`).
*   **Stack Data Structure:** Leverages native `Stack<T>` collections in C# to parse tokens and pop results with $O(N)$ time complexity efficiency.

---

## 🏗️ Technical Stack & Architecture

*   **Language:** C# (.NET Framework / .NET Core WinForms)
*   **UI Paradigm:** Custom Control Architecture & Component Inheritance
*   **Data Structures:** Stacks, Queues, and Tokenization Parsing Trees
*   **IDE:** Visual Studio 2022

---

## 🛠️ How the Engine Works (Quick Overview)

1.  **Tokenization:** The custom display collects input strings as individual tokens (Numbers vs. Operators).
2.  **Notation Conversion:** The business logic re-orders the tokens into **Prefix / Postfix (Polish Notation)** to eliminate operational ambiguity.
3.  **Stack Evaluation:** The evaluation engine loops through the rearranged stack, computing values sequentially and preventing common order-of-operation bugs.

---

## 🔧 Installation & Running Locally

### Prerequisites
*   Visual Studio 2022 with the **.NET Desktop Development** workload installed.

### Setup Steps
1.  Clone this repository to your local machine:
```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  Open the `.sln` (Solution) file inside Visual Studio.
3.  Press `F5` or click **Start** to build and run the desktop application.
