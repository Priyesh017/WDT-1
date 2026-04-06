# Modern DOM Calculator

A modern, responsive calculator built entirely using Vanilla JavaScript DOM manipulation and styled with Tailwind CSS. This project was developed to demonstrate dynamic element creation, event delegation, strict keyboard event handling, and data persistence.

## 🚀 Features

- **100% DOM-Generated UI:** The HTML `<body>` is kept completely empty. Every structural element, display screen, and button is dynamically generated using `document.createElement()`.
- **Modern Neumorphic-Inspired UI:** Styled utilizing Tailwind CSS for a responsive, clean, and interactive design with hover and active states.
- **Smart Keyboard Handling:** \* Allows keyboard input strictly for numbers (`0-9`).
  - Triggers an explicit `alert("Only numbers are allowed")` if the user attempts to type letters or mathematical operators via the keyboard, ensuring strict input validation.
- **State Persistence:** Utilizes `localStorage` to save the current state of the calculation. If the page is refreshed or accidentally closed, the user's progress is fully restored.
- **Advanced Calculator Logic:**
  - **Infix Expression Evaluation:** Safely handles standard math strings (e.g., `5 + 5 * 2`) using JavaScript's native evaluation.
  - **Consecutive Operator Prevention:** Prevents syntax errors by automatically replacing old operators if multiple are clicked in a row (e.g., clicking `+` then `-` results in just `-`).
  - **Smart Zero Handling:** Prevents invalid number strings like `05` by safely replacing starting zeros.
  - **Visual Formatting:** Dynamically scales down mathematical operators (`+`, `-`, `X`, `/`, `%`) on the display screen for better readability.

## 🛠️ Technologies Used

- **HTML5:** Skeleton structure and script importing.
- **Vanilla JavaScript (ES6+):** Core logic, DOM manipulation, Regular Expressions, and Event Listeners.
- **Tailwind CSS:** Utility-first CSS framework via CDN for rapid styling and responsiveness.

## 💻 How to Run the Project

Since this project uses entirely front-end technologies with no build steps, running it is incredibly simple:

1. Clone or download this repository to your local machine.
2. Ensure you have an active internet connection (required to fetch the Tailwind CSS CDN).
3. Open the `index.html` file in any modern web browser (Chrome, Firefox, Edge, Safari).

## 📝 Assignment Requirements Met

This project was built to satisfy the following specific constraints:

1. **Use DOM to create HTML elements:** Met via JavaScript-only rendering.
2. **Use Keyboard events only for numbers:** Met via the `keydown` event listener strictly checking `/^[0-9]$/`.
3. **Alert warning for non-numbers:** Triggered automatically via the keyboard event logic.
4. **Specific operations (+, -, /, \*, %):** All included and functional.
5. **Handle infix expressions:** Handled correctly before evaluation.
6. **Responsive UI with CSS/Bootstrap:** Met using Tailwind CSS.
7. **Test Suite Included:** ZenClass test suite script is attached at the bottom of the document.
