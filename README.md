# increment-decrement-counter

The Increment Decrement Counter is a straightforward web application built using HTML, CSS, and JavaScript. It provides users with the ability to increment or decrement a numeric value using intuitive buttons. The project is designed to be responsive, ensuring a consistent user experience across various screen sizes.

Features
Increment and decrement buttons to adjust the numeric value.
A responsive layout that works well on different devices and screen sizes.
Getting Started
Follow these steps to set up the Increment Decrement Counter on your local machine.

Prerequisites
You'll need a modern web browser that supports HTML5, CSS3, and JavaScript.



Responsive Design
The Increment Decrement Counter is designed with responsiveness in mind. This is accomplished using CSS media queries to adjust the layout and styling based on the screen size. The CSS rules ensure that the counter remains usable and visually appealing on various devices.


JavaScript Logic
The JavaScript logic for the Increment Decrement Counter revolves around managing the displayed value and handling button clicks:


// Get references to HTML elements
const valueElement = document.getElementById('value');
const incrementButton = document.getElementById('increment');
const decrementButton = document.getElementById('decrement');

let currentValue = 0;

// Update the value element with the current value
function updateValue() {
  valueElement.textContent = currentValue;
}

// Increment the value and update the display
incrementButton.addEventListener('click', () => {
  currentValue++;
  updateValue();
});

// Decrement the value and update the display
decrementButton.addEventListener('click', () => {
  if (currentValue > 0) {
    currentValue--;
    updateValue();
  }
});

// Initialize the value display
updateValue();
