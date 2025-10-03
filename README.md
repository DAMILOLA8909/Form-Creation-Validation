# Form-Creation-Validation
ALX week 6 activity on JavaScript Deep dive.

# Form Creation & Validation 📝

A simple web project for client-side form validation using plain JavaScript.  
This repository is part of **ALX Week 6** (JavaScript Deep Dive) assignment.  
Validates user input (username, email, password) and provides instant feedback.

---

## 📁 Repository Structure

Form-Creation-Validation/
│

├── index.html # The HTML form

├── style.css # Basic styling for form & feedback

├── script.js # JavaScript validation logic

└── README.md # This document


---

## ✅ Features & Validation Rules

- The form includes **Username**, **Email**, and **Password** fields.
- On submit, JavaScript intercepts the form (prevents actual submission) and validates:
  1. **Username** must be at least **3 characters** long.
  2. **Email** must contain both `@` and `.` (a basic check).
  3. **Password** must be at least **8 characters** long.
- If **all validations pass**, a success message is shown.
- If **any validation fails**, error messages are shown (one per problem).
- Feedback (success or error) is displayed in a styled `div` below the form.

---

## 🧪 How It Works

1. The script runs after the page is fully loaded (via `DOMContentLoaded`).
2. It grabs references to the form (`#registration-form`) and feedback container (`#form-feedback`).
3. On submit:
   - Prevent default behavior (`event.preventDefault()`).
   - Read and `.trim()` each input.
   - Perform checks; collect error messages if any.
   - Display feedback: green success or red errors, using innerHTML/textContent and color styling.

---

## 🚀 Getting Started / Usage

1. Clone this repo:

   ```bash
   git clone https://github.com/DAMILOLA8909/Form-Creation-Validation

2. Open index.html in your browser (no build step required).

3. Try entering invalid and valid inputs to see live feedback.
