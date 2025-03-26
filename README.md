# Dev-Tools-Tricks

This project demonstrates various **JavaScript Console Tricks** that can be used to debug, style, and analyze data while developing web applications. The code includes examples of different `console` methods and a fun interactive feature to dynamically change the appearance of a DOM element.

---

## Features

### Interactive DOM Manipulation
- Clicking the text `xBREAKxDOWNx` changes its:
  - **Color** to `#BADA55`.
  - **Font size** to `50px`.

### Console Tricks
The following console methods are showcased:

1. **Regular Logs**
   - Example: `console.log('Hello!');`

2. **Interpolated Strings**
   - Example: `console.log('Hello! I am a %s string', '🧑');`

3. **Styled Logs**
   - Example: `console.log('%cHello! I am a styled text', 'font-size: 24px; background: red');`

4. **Warnings**
   - Example: `console.warn('Be Careful!');`

5. **Errors**
   - Example: `console.error('Error!');`

6. **Information**
   - Example: `console.info('Apple a day keeps doctor away!');`

7. **Assertions**
   - Tests a condition and logs a message if the assertion fails.
   - Example: `console.assert(p.classList.contains('ouuch'), 'That is wrong');`

8. **Clearing Console**
   - Uncomment `console.clear();` to clear the console.

9. **Viewing DOM Elements**
   - Logs the selected DOM element with `console.log(p);` or `console.dir(p);`.

10. **Grouping**
    - Groups related logs together.
    - Example: Groups data for `dogs` using `console.groupCollapsed()` and `console.groupEnd()`.

11. **Counting**
    - Tracks how many times a label has been logged.
    - Example:
      ```javascript
      console.count('Tanzim');
      console.count('Ikram');
      ```

12. **Timing**
    - Measures how long an operation takes.
    - Example:
      ```javascript
      console.time('fetching data');
      fetch('https://api.github.com/users/wesbos')
      .then(data => data.json())
      .then(data => {
          console.timeEnd('fetching data');
          console.log(data);
      });
      ```

13. **Tables**
    - Logs an array of objects as a table.
    - Example: `console.table(dogs);`

---

## How to Run

1. Open the `index.html` file in any browser.
2. Open the **Developer Tools** in your browser (usually accessible with `F12` or `Ctrl+Shift+I`).
3. View the console to see the examples in action.
4. Click on the `xBREAKxDOWNx` text to see the interactive feature.

---

## Learning Objectives

This project helps you:
- Explore the wide range of JavaScript `console` methods.
- Understand how to interact with and manipulate the DOM.
- Learn how to debug efficiently using the browser's developer tools.