🎨 Color Scheme Switcher

A simple JavaScript-based color scheme switcher that allows users to change the background color of a webpage by clicking on colored buttons.

📌 Features

Clickable color buttons (Grey, White, Blue, Red)

Instantly changes the background color of the page

Clean and responsive layout

Beginner-friendly HTML, CSS, and JavaScript

Includes a function to generate random colors (optional / extendable)

🛠️ Technologies Used

HTML5 – Structure of the page

CSS3 – Styling and layout

JavaScript (ES6) – DOM manipulation and event handling

📂 Project Structure
color-scheme-switcher/
│
├── index.html
└── README.md

🚀 How It Works

The page displays colored square buttons.

Each button has a unique id representing a color.

JavaScript listens for click events on these buttons.

When clicked, the page background changes to the selected color.

🧠 Key JavaScript Logic
let btn = document.querySelectorAll('.button');
const body = document.querySelector('body');

btn.forEach(button => {
    button.addEventListener('click', (e) => {
        body.style.backgroundColor = e.target.id;
    });
});
