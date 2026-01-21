# 🧮 Calculator

A modern, responsive web-based calculator built with vanilla HTML, CSS, and JavaScript. This calculator provides a clean user interface with essential arithmetic operations and a user-friendly design.

[![HTML](https://img.shields.io/badge/HTML-52.8%25-orange)](https://github.com/Allanagari-Renuka/Calculator)
[![CSS](https://img.shields.io/badge/CSS-33.2%25-blue)](https://github.com/Allanagari-Renuka/Calculator)
[![JavaScript](https://img.shields.io/badge/JavaScript-14.0%25-yellow)](https://github.com/Allanagari-Renuka/Calculator)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Code Overview](#code-overview)
- [Customization](#customization)
- [Browser Support](#browser-support)
- [Contributing](#contributing)
- [Future Enhancements](#future-enhancements)
- [License](#license)
- [Author](#author)

## 🎯 Overview

This calculator is a lightweight, browser-based application that performs standard arithmetic operations. Built without any external dependencies, it showcases clean code practices and modern web development techniques using pure HTML5, CSS3, and vanilla JavaScript.

Perfect for:
- Learning web development fundamentals
- Understanding DOM manipulation
- Exploring CSS styling techniques
- Building a portfolio project
- Quick calculations in the browser

## ✨ Features

### Core Functionality
- ➕ **Addition** - Add multiple numbers
- ➖ **Subtraction** - Subtract values
- ✖️ **Multiplication** - Multiply numbers
- ➗ **Division** - Divide with precision
- 🔢 **Decimal Support** - Handle floating-point numbers
- 🔄 **Clear Function** - Reset calculations instantly
- ⌫ **Backspace/Delete** - Remove last digit

### User Experience
- 🎨 **Modern UI Design** - Clean and intuitive interface
- 📱 **Responsive Layout** - Works on all device sizes
- ⌨️ **Keyboard Support** - Use number keys and operators
- 🖱️ **Click-friendly Buttons** - Large, easy-to-press buttons
- 🎯 **Real-time Display** - Instant feedback on operations
- 🚫 **Error Handling** - Prevents invalid operations

### Design Features
- Smooth transitions and animations
- Hover effects for better interactivity
- Clear visual feedback for button presses
- Professional color scheme
- Readable font and spacing

## 🚀 Demo

### Quick Start
Simply open `calculator.html` in any modern web browser to start using the calculator!

### Screenshots
```
┌─────────────────────────┐
│      Calculator         │
├─────────────────────────┤
│  Display Screen         │
│  ┌──────────────────┐  │
│  │         0        │  │
│  └──────────────────┘  │
├─────────────────────────┤
│  [7] [8] [9] [÷]       │
│  [4] [5] [6] [×]       │
│  [1] [2] [3] [-]       │
│  [0] [.] [=] [+]       │
│  [C] [←]               │
└─────────────────────────┘
```

## 🛠️ Technologies Used

### Frontend
- **HTML5** - Semantic markup and structure
- **CSS3** - Modern styling and animations
  - Flexbox/Grid for layout
  - CSS Variables for theming
  - Media queries for responsiveness
  - Transitions for smooth effects
- **JavaScript (ES6+)** - Core functionality and logic
  - DOM manipulation
  - Event listeners
  - Mathematical operations
  - Input validation

### Development Tools
- Any modern text editor (VS Code, Sublime Text, Atom)
- Web browser with developer tools
- Git for version control

## 📥 Installation

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Basic understanding of HTML/CSS/JavaScript (for customization)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Allanagari-Renuka/Calculator.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd Calculator
   ```

3. **Open in browser**
   
   **Option A: Direct Opening**
   ```bash
   # Simply double-click calculator.html
   # Or right-click → Open with → Your Browser
   ```

   **Option B: Using Live Server**
   ```bash
   # If using VS Code with Live Server extension
   # Right-click on calculator.html → Open with Live Server
   ```

   **Option C: Using Python HTTP Server**
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   
   # Then open http://localhost:8000/calculator.html
   ```

4. **Start calculating!** 🎉

## 💻 Usage

### Basic Operations

1. **Entering Numbers**
   - Click number buttons (0-9) or use keyboard
   - Build multi-digit numbers by clicking sequentially

2. **Performing Calculations**
   - Click an operator (+, -, ×, ÷)
   - Enter the second number
   - Press '=' or Enter key to see the result

3. **Using Decimal Points**
   - Click '.' button to add decimal
   - Only one decimal point per number is allowed

4. **Clearing**
   - **C button**: Clears entire calculation
   - **← button**: Removes last digit (backspace)

5. **Keyboard Shortcuts**
   - `0-9`: Number input
   - `+`: Addition
   - `-`: Subtraction
   - `*`: Multiplication
   - `/`: Division
   - `Enter` or `=`: Calculate result
   - `Escape` or `C`: Clear all
   - `Backspace`: Delete last character
   - `.`: Decimal point

### Example Calculations

```
Addition:        25 + 30 = 55
Subtraction:     100 - 45 = 55
Multiplication:  12 × 5 = 60
Division:        100 ÷ 4 = 25
Decimals:        5.5 + 2.3 = 7.8
Complex:         (15 + 5) × 2 = 40
```

## 📁 File Structure

```
Calculator/
│
├── calculator.html        # Main HTML structure
├── calculator.css         # Styling and layout
├── calculator.js          # Core functionality and logic
└── README.md             # Documentation (this file)
```

### File Descriptions

**calculator.html**
- Contains the HTML structure
- Defines the calculator layout
- Links CSS and JavaScript files
- Includes semantic markup

**calculator.css**
- All styling rules
- Responsive design breakpoints
- Button styles and animations
- Display screen formatting
- Color scheme and typography

**calculator.js**
- Event listeners for buttons
- Calculation logic
- Input validation
- Display updates
- Error handling
- Keyboard input processing

## 🔍 Code Overview

### HTML Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="calculator.css">
</head>
<body>
    <div class="calculator">
        <div class="display"></div>
        <div class="buttons">
            <!-- Number and operator buttons -->
        </div>
    </div>
    <script src="calculator.js"></script>
</body>
</html>
```

### CSS Highlights
```css
/* Modern styling with CSS Grid/Flexbox */
.calculator {
    display: grid;
    width: 100%;
    max-width: 400px;
    margin: 0 auto;
}

/* Responsive button layout */
.buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

/* Smooth animations */
button:active {
    transform: scale(0.95);
    transition: transform 0.1s;
}
```

### JavaScript Architecture
```javascript
// Core calculation logic
let currentNumber = '';
let previousNumber = '';
let operation = null;

function calculate() {
    // Perform arithmetic operations
    // Handle edge cases
    // Update display
}

// Event listeners
buttons.forEach(button => {
    button.addEventListener('click', handleButtonClick);
});
```

## 🎨 Customization

### Changing Colors

Edit `calculator.css`:
```css
:root {
    --primary-color: #4CAF50;     /* Change button colors */
    --secondary-color: #2196F3;   /* Change operator colors */
    --background: #f5f5f5;        /* Change background */
    --text-color: #333;           /* Change text color */
}
```

### Modifying Button Sizes

```css
.button {
    width: 80px;      /* Adjust width */
    height: 80px;     /* Adjust height */
    font-size: 24px;  /* Adjust font size */
}
```

### Adding New Features

**Example: Adding a Square Root Function**

1. Add button in HTML:
```html
<button class="operator" data-action="sqrt">√</button>
```

2. Add logic in JavaScript:
```javascript
case 'sqrt':
    currentNumber = Math.sqrt(parseFloat(currentNumber));
    updateDisplay();
    break;
```

3. Style in CSS:
```css
button[data-action="sqrt"] {
    background-color: #9C27B0;
}
```

## 🌐 Browser Support

| Browser | Version | Supported |
|---------|---------|-----------|
| Chrome  | 90+     | ✅ Yes    |
| Firefox | 88+     | ✅ Yes    |
| Safari  | 14+     | ✅ Yes    |
| Edge    | 90+     | ✅ Yes    |
| Opera   | 76+     | ✅ Yes    |

### Mobile Browsers
- iOS Safari 14+
- Chrome Mobile 90+
- Firefox Mobile 88+
- Samsung Internet 14+

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Reporting Bugs
1. Check if the bug has already been reported in [Issues](https://github.com/Allanagari-Renuka/Calculator/issues)
2. Create a new issue with:
   - Clear title and description
   - Steps to reproduce
   - Expected vs actual behavior
   - Screenshots if applicable

### Submitting Changes

1. **Fork the repository**
   ```bash
   git fork https://github.com/Allanagari-Renuka/Calculator.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Make your changes**
   - Follow existing code style
   - Comment complex logic
   - Test thoroughly

4. **Commit your changes**
   ```bash
   git commit -m "Add: Amazing new feature"
   ```

5. **Push to your branch**
   ```bash
   git push origin feature/AmazingFeature
   ```

6. **Open a Pull Request**
   - Describe your changes clearly
   - Reference any related issues
   - Include screenshots for UI changes

### Code Style Guidelines
- Use meaningful variable names
- Add comments for complex logic
- Follow consistent indentation (2 or 4 spaces)
- Keep functions small and focused
- Write semantic HTML
- Use CSS classes instead of IDs for styling

## 🚀 Future Enhancements

### Planned Features
- [ ] **Scientific Mode**
  - Trigonometric functions (sin, cos, tan)
  - Logarithmic functions (log, ln)
  - Exponents and powers
  - Square root and nth root
  
- [ ] **History Feature**
  - Save calculation history
  - Review past calculations
  - Clear history option

- [ ] **Themes**
  - Dark mode toggle
  - Multiple color schemes
  - Custom theme builder

- [ ] **Advanced Features**
  - Memory functions (M+, M-, MR, MC)
  - Percentage calculations
  - Parentheses support for complex expressions
  - Copy result to clipboard

- [ ] **Accessibility**
  - Screen reader support
  - High contrast mode
  - Keyboard navigation improvements
  - ARIA labels

- [ ] **Mobile Enhancements**
  - Native app wrapper
  - Haptic feedback
  - Portrait/landscape optimization

### Want to Implement a Feature?
Check the [Issues](https://github.com/Allanagari-Renuka/Calculator/issues) page or create a new feature request!

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary
```
Permission is granted to use, copy, modify, merge, publish, distribute,
sublicense, and/or sell copies of the software, subject to including
the copyright notice and permission notice in all copies.
```

## 👤 Author

**Renuka Allanagari**

- GitHub: [@Allanagari-Renuka](https://github.com/Allanagari-Renuka)
- LinkedIn: [Add your LinkedIn profile]
- Email: [Add your email]
- Portfolio: [Add your portfolio website]

## 🙏 Acknowledgments

- Thanks to the open-source community for inspiration
- Built with passion for learning and sharing knowledge
- Special thanks to all contributors

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/Allanagari-Renuka/Calculator/issues) page
2. Create a new issue with details
3. Reach out to the author

## 🌟 Show Your Support

If you found this project helpful or learned something from it:

- ⭐ Star this repository
- 🔀 Fork it for your own projects
- 📢 Share it with others
- 🐛 Report bugs
- 💡 Suggest new features
