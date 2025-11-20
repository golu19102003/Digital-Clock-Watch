<img width="512" height="215" alt="image" src="https://github.com/user-attachments/assets/8ef091d9-0687-4007-9170-c0abd0554ced" />

# Digital-Clock-Watch
⏰ Web Clock Watch
A simple and responsive digital clock built using HTML, CSS, and JavaScript. This project displays the current time in hours, minutes, and seconds, updating in real time. It is ideal for beginners learning DOM manipulation, styling, and basic JavaScript functions.

## 📌 Features:

⏱️ Real-time digital clock

🎨 Clean and minimal UI

📱 Fully responsive design

⚡ Uses basic JavaScript without any external libraries

🌙 Easy to customize (colors, fonts, layout)

## 📁 Project Structure:
web-clock/;
│── index.html   # Main HTML structure
│── style.css    # Clock styling
└── script.js    # Logic for real-time clock updates

## 🚀 How It Works:

HTML defines the layout for displaying the time.

CSS adds styling for alignment, fonts, and visual design.

JavaScript uses setInterval() to:

Get the current system time

Format hours, minutes, and seconds

Update the clock display every second

## ▶️ How to Run the Project:

Download or clone the project folder

Open index.html in any modern web browser

The clock will start running automatically

🧩 Sample Code
**index.html**
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Web Clock</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="clock"></div>
    <script src="script.js"></script>
</body>
</html>

**style.css**
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: #000;
    margin: 0;
    font-family: Arial, sans-serif;
}

#clock {
    color: #00ff99;
    font-size: 70px;
    letter-spacing: 3px;
}

**script.js**
function updateClock() {
    const now = new Date();
    const time = now.toLocaleTimeString();
    document.getElementById("clock").textContent = time;
}

setInterval(updateClock, 1000);
updateClock();
