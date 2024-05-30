# Simple Calculator

This project is a simple calculator built using HTML, CSS, and JavaScript. The calculator provides basic arithmetic operations such as addition, subtraction, multiplication, and division. The user interface is designed with a modern aesthetic, using the Orbitron font and a color scheme that is both visually appealing and functional.

## Features

- **Basic Arithmetic Operations**: Perform addition, subtraction, multiplication, and division.
- **Clear Screen Functionality**: Clear the current input to start a new calculation.
- **Responsive Design**: The calculator is designed to be used on various device sizes.
- **User-Friendly Interface**: Intuitive button layout with distinct color coding for operations and results.

## Files Included

1. **index.html**: The main HTML file that contains the structure of the calculator.
2. **styles.css**: The CSS file that styles the calculator.
3. **script.js**: The JavaScript file that contains the functionality of the calculator.

## How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/simple-calculator.git
   ```
2. **Open the Project**
   Navigate to the project directory and open the `index.html` file in your web browser.

## Detailed File Descriptions

### index.html

This is the main HTML file that structures the calculator interface using a table layout. Each button is an HTML input element with type "button", which triggers specific JavaScript functions on click.

### styles.css

This CSS file styles the calculator, providing it with a sleek and modern look. Key styling features include:

- **Calculator Container**: `.calculator` class styles the main container with padding, rounded corners, background color, and shadow.
- **Display Box**: `.display-box` class styles the display area where the calculation results are shown.
- **Buttons**: `input[type=button]` styles all the buttons with a consistent look and feel, including background color, border, and font.

### script.js

This JavaScript file provides the interactive functionality of the calculator. It includes three main functions:

- **clearScreen()**: Clears the display.
  ```javascript
  function clearScreen() {
      document.getElementById("result").value = "";
  }
  ```
- **display(value)**: Appends the clicked button's value to the display.
  ```javascript
  function display(value) {
      document.getElementById("result").value += value;
  }
  ```
- **calculate()**: Evaluates the expression in the display and shows the result.
  ```javascript
  function calculate() {
      var p = document.getElementById("result").value;
      var q = eval(p);
      document.getElementById("result").value = q;
  }
  ```

## How It Works

- When a number or operator button is clicked, the `display(value)` function adds the respective value to the display.
- The "C" button calls the `clearScreen()` function, which clears the display.
- The "=" button calls the `calculate()` function, which uses JavaScript's `eval()` function to evaluate the mathematical expression in the display and then updates the display with the result.

## Customization

You can customize the calculator by:

- Changing the colors in `styles.css` to match your preferred color scheme.
- Adding more advanced functions (like square root, exponentiation) by extending the JavaScript code in `script.js`.

## Fonts

The calculator uses the "Orbitron" font from Google Fonts. Ensure you have internet connectivity to load the font, or you can download and host it locally.

## License

This project is open source and available under the [MIT License](LICENSE).

## Conclusion

This simple calculator project is an excellent starting point for beginners learning web development with HTML, CSS, and JavaScript. It covers basic UI design and interactive functionality, providing a foundation for more advanced projects.