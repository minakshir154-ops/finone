# finone
universal super wallet
<!DOCTYPE html>

<html lang="en">

<head>

  <meta charset="UTF-8" />

  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>FinOne - Universal Super Wallet</title>

  <link rel="stylesheet" href="style.css" />

  <link rel="icon" type="image/png" href="logo.png" />

</head>

<body>

  <!-- Splash Screen with Animated SVG -->

  <div id="splash">

    <div class="svg-wrapper">

      <svg width="110" height="110" viewBox="0 0 110 110" xmlns="http://www.w3.org/2000/svg">

        <defs>

          <linearGradient id="grad" x1="0%" y1="0%" x2="100%" y2="100%">

            <stop offset="0%" style="stop-color:#004aad;stop-opacity:1" />

            <stop offset="100%" style="stop-color:#00b4d8;stop-opacity:1" />

          </linearGradient>

        </defs>

        <circle cx="55" cy="55" r="50" stroke="url(#grad)" stroke-width="5" fill="none" class="spin-circle"/>

        <text x="50%" y="55%" dominant-baseline="middle" text-anchor="middle" font-size="22" font-weight="bold" fill="url(#grad)">₹</text>

      </svg>

    </div>

    <h1 class="splash-text">FinOne</h1>

    <p class="splash-sub">Finance for Everyone, Everywhere</p>

  </div>

  <!-- Header -->

  <header>

    <div class="logo-area">

      <img src="logo.png" alt="FinOne Logo" class="logo-img">

    </div>

    <nav class="desktop-nav">

      <a href="#dashboard">Dashboard</a>

      <a href="#voice">Assistant</a>

      <a href="#goals">Goals</a>

      <a href="#contact">Join</a>

    </nav>

    <div class="toggle-container">

      <input type="checkbox" id="themeToggle" />

      <label for="themeToggle" class="toggle-label">

        🌞 <span class="toggle-slider"></span> 🌙

      </label>

    </div>

  </header>

  <main id="app-content" class="hidden">

    <!-- Dashboard -->

    <section id="dashboard" class="dashboard active-screen">

      <h2>📊 FinOne Dashboard</h2>

      <div class="dashboard-grid">

        <div class="dash-card balance">

          <h3>Wallet Balance</h3>

          <p class="amount">₹4,250</p>

          <button class="refresh-btn" id="refreshBalance">🔄 Refresh</button>

        </div>

        <div class="dash-card transactions">

          <h3>Recent Transactions</h3>

          <ul id="txList">

            <li>✅ Sent ₹500 to Rahul Kumar</li>

            <li>💰 Received ₹1,200 from Priya</li>

            <li>☕ Paid ₹150 at Café Mocha</li>

          </ul>

        </div>

        <div class="dash-card goals">

          <h3>My Goals</h3>

          <p id="goalSummary">🎯 Save ₹10,000 for Phone</p>

        </div>

        <div class="dash-card ai-summary">

          <h3>AI Insights</h3>

          <p id="aiInsight">Your weekly savings grew by 15%. Great job!</p>

          <button id="askAI">Ask AI Insight</button>

        </div>

      </div>

    </section>

    <!-- Voice Assistant -->

    <section id="voice" class="voice-assistant hidden-screen">

      <h2>🎙 FinOne Voice Assistant</h2>

      <p>Try saying “Send ₹500 to my son.”</p>

      <div class="assistant-box">

        <input type="text" id="voiceInput" placeholder="Say or type your command..." />

        <button id="sendCommand">Send</button>

      </div>

      <div id="response" class="response-box"></div>

    </section>

    <!-- Smart Goals -->

    <section id="goals" class="smart-goals hidden-screen">

      <h2>🎯 Smart Savings Goals</h2>

      <p>Set goals with voice or text. Example: “Save ₹10,000 for phone.”</p>

      <div class="goal-box">

        <input type="text" id="goalInput" placeholder="Enter your goal..." />

        <button id="saveGoal">Set Goal</button>

      </div>

      <div id="goalDisplay" class="goal-display"></div>

    </section>

  </main>

  <!-- Floating Mic -->

  <button id="floatMic" class="float-mic">🎤</button>

  <!-- Bottom Navigation -->

  <div class="bottom-nav">

    <button data-target="dashboard">🏠</button>

    <button data-target="voice">💬</button>

    <button data-target="goals">🎯</button>

    <button data-target="contact">👤</button>

  </div>

  <footer id="contact">

    <p>🌍 FinOne © 2025 | Building Inclusive Finance for Every Indian</p>

  </footer>

  <script src="script.js"></script>

</body>

</html><!DOCTYPE html>

<html lang="en">

<head>

  <meta charset="UTF-8" />

  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>FinOne - Universal Super Wallet</title>

  <link rel="stylesheet" href="style.css" />

  <link rel="icon" type="image/png" href="logo.png" />

</head>

<body>

  <!-- Splash Screen with Animated SVG -->

  <div id="splash">

    <div class="svg-wrapper">

      <svg width="110" height="110" viewBox="0 0 110 110" xmlns="http://www.w3.org/2000/svg">

        <defs>

          <linearGradient id="grad" x1="0%" y1="0%" x2="100%" y2="100%">

            <stop offset="0%" style="stop-color:#004aad;stop-opacity:1" />

            <stop offset="100%" style="stop-color:#00b4d8;stop-opacity:1" />

          </linearGradient>

        </defs>

        <circle cx="55" cy="55" r="50" stroke="url(#grad)" stroke-width="5" fill="none" class="spin-circle"/>

        <text x="50%" y="55%" dominant-baseline="middle" text-anchor="middle" font-size="22" font-weight="bold" fill="url(#grad)">₹</text>

      </svg>

    </div>

    <h1 class="splash-text">FinOne</h1>

    <p class="splash-sub">Finance for Everyone, Everywhere</p>

  </div>

  <!-- Header -->

  <header>

    <div class="logo-area">

      <img src="logo.png" alt="FinOne Logo" class="logo-img">

    </div>

    <nav class="desktop-nav">

      <a href="#dashboard">Dashboard</a>

      <a href="#voice">Assistant</a>

      <a href="#goals">Goals</a>

      <a href="#contact">Join</a>

    </nav>

    <div class="toggle-container">

      <input type="checkbox" id="themeToggle" />

      <label for="themeToggle" class="toggle-label">

        🌞 <span class="toggle-slider"></span> 🌙

      </label>

    </div>

  </header>

  <main id="app-content" class="hidden">

    <!-- Dashboard -->

    <section id="dashboard" class="dashboard active-screen">

      <h2>📊 FinOne Dashboard</h2>

      <div class="dashboard-grid">

        <div class="dash-card balance">

          <h3>Wallet Balance</h3>

          <p class="amount">₹4,250</p>

          <button class="refresh-btn" id="refreshBalance">🔄 Refresh</button>

        </div>

        <div class="dash-card transactions">

          <h3>Recent Transactions</h3>

          <ul id="txList">

            <li>✅ Sent ₹500 to Rahul Kumar</li>

            <li>💰 Received ₹1,200 from Priya</li>

            <li>☕ Paid ₹150 at Café Mocha</li>

          </ul>

        </div>

        <div class="dash-card goals">

          <h3>My Goals</h3>

          <p id="goalSummary">🎯 Save ₹10,000 for Phone</p>

        </div>

        <div class="dash-card ai-summary">

          <h3>AI Insights</h3>

          <p id="aiInsight">Your weekly savings grew by 15%. Great job!</p>

          <button id="askAI">Ask AI Insight</button>

        </div>

      </div>

    </section>

    <!-- Voice Assistant -->

    <section id="voice" class="voice-assistant hidden-screen">

      <h2>🎙 FinOne Voice Assistant</h2>

      <p>Try saying “Send ₹500 to my son.”</p>

      <div class="assistant-box">

        <input type="text" id="voiceInput" placeholder="Say or type your command..." />

        <button id="sendCommand">Send</button>

      </div>

      <div id="response" class="response-box"></div>

    </section>

    <!-- Smart Goals -->

    <section id="goals" class="smart-goals hidden-screen">

      <h2>🎯 Smart Savings Goals</h2>

      <p>Set goals with voice or text. Example: “Save ₹10,000 for phone.”</p>

      <div class="goal-box">

        <input type="text" id="goalInput" placeholder="Enter your goal..." />

        <button id="saveGoal">Set Goal</button>

      </div>

      <div id="goalDisplay" class="goal-display"></div>

    </section>

  </main>

  <!-- Floating Mic -->

  <button id="floatMic" class="float-mic">🎤</button>

  <!-- Bottom Navigation -->

  <div class="bottom-nav">

    <button data-target="dashboard">🏠</button>

    <button data-target="voice">💬</button>

    <button data-target="goals">🎯</button>

    <button data-target="contact">👤</button>

  </div>

  <footer id="contact">

    <p>🌍 FinOne © 2025 | Building Inclusive Finance for Every Indian</p>

  </footer>

  <script src="script.js"></script>

</body>

</html><!DOCTYPE html>

<html lang="en">

<head>

  <meta charset="UTF-8" />

  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>FinOne - Universal Super Wallet</title>

  <link rel="stylesheet" href="style.css" />

  <link rel="icon" type="image/png" href="logo.png" />

</head>

<body>

  <!-- Splash Screen with Animated SVG -->

  <div id="splash">

    <div class="svg-wrapper">

      <svg width="110" height="110" viewBox="0 0 110 110" xmlns="http://www.w3.org/2000/svg">

        <defs>

          <linearGradient id="grad" x1="0%" y1="0%" x2="100%" y2="100%">

            <stop offset="0%" style="stop-color:#004aad;stop-opacity:1" />

            <stop offset="100%" style="stop-color:#00b4d8;stop-opacity:1" />

          </linearGradient>

        </defs>

        <circle cx="55" cy="55" r="50" stroke="url(#grad)" stroke-width="5" fill="none" class="spin-circle"/>

        <text x="50%" y="55%" dominant-baseline="middle" text-anchor="middle" font-size="22" font-weight="bold" fill="url(#grad)">₹</text>

      </svg>

    </div>

    <h1 class="splash-text">FinOne</h1>

    <p class="splash-sub">Finance for Everyone, Everywhere</p>

  </div>

  <!-- Header -->

  <header>

    <div class="logo-area">

      <img src="logo.png" alt="FinOne Logo" class="logo-img">

    </div>

    <nav class="desktop-nav">

      <a href="#dashboard">Dashboard</a>

      <a href="#voice">Assistant</a>

      <a href="#goals">Goals</a>

      <a href="#contact">Join</a>

    </nav>

    <div class="toggle-container">

      <input type="checkbox" id="themeToggle" />

      <label for="themeToggle" class="toggle-label">

        🌞 <span class="toggle-slider"></span> 🌙

      </label>

    </div>

  </header>

  <main id="app-content" class="hidden">

    <!-- Dashboard -->

    <section id="dashboard" class="dashboard active-screen">

      <h2>📊 FinOne Dashboard</h2>

      <div class="dashboard-grid">

        <div class="dash-card balance">

          <h3>Wallet Balance</h3>

          <p class="amount">₹4,250</p>

          <button class="refresh-btn" id="refreshBalance">🔄 Refresh</button>

        </div>

        <div class="dash-card transactions">

          <h3>Recent Transactions</h3>

          <ul id="txList">

            <li>✅ Sent ₹500 to Rahul Kumar</li>

            <li>💰 Received ₹1,200 from Priya</li>

            <li>☕ Paid ₹150 at Café Mocha</li>

          </ul>

        </div>

        <div class="dash-card goals">

          <h3>My Goals</h3>

          <p id="goalSummary">🎯 Save ₹10,000 for Phone</p>

        </div>

        <div class="dash-card ai-summary">

          <h3>AI Insights</h3>

          <p id="aiInsight">Your weekly savings grew by 15%. Great job!</p>

          <button id="askAI">Ask AI Insight</button>

        </div>

      </div>

    </section>

    <!-- Voice Assistant -->

    <section id="voice" class="voice-assistant hidden-screen">

      <h2>🎙 FinOne Voice Assistant</h2>

      <p>Try saying “Send ₹500 to my son.”</p>

      <div class="assistant-box">

        <input type="text" id="voiceInput" placeholder="Say or type your command..." />

        <button id="sendCommand">Send</button>

      </div>

      <div id="response" class="response-box"></div>

    </section>

    <!-- Smart Goals -->

    <section id="goals" class="smart-goals hidden-screen">

      <h2>🎯 Smart Savings Goals</h2>

      <p>Set goals with voice or text. Example: “Save ₹10,000 for phone.”</p>

      <div class="goal-box">

        <input type="text" id="goalInput" placeholder="Enter your goal..." />

        <button id="saveGoal">Set Goal</button>

      </div>

      <div id="goalDisplay" class="goal-display"></div>

    </section>

  </main>

  <!-- Floating Mic -->

  <button id="floatMic" class="float-mic">🎤</button>

  <!-- Bottom Navigation -->

  <div class="bottom-nav">

    <button data-target="dashboard">🏠</button>

    <button data-target="voice">💬</button>

    <button data-target="goals">🎯</button>

    <button data-target="contact">👤</button>

  </div>

  <footer id="contact">

    <p>🌍 FinOne © 2025 | Building Inclusive Finance for Every Indian</p>

  </footer>

  <script src="script.js"></script>

</body>

</html>
:root {

  --primary: #004aad;

  --secondary: #00b4d8;

  --text: #222;

  --bg: #f4f7fb;

  --card-bg: white;

}

body.dark {

  --primary: #00b4d8;

  --secondary: #004aad;

  --text: #f1f1f1;

  --bg: #0d1117;

  --card-bg: #161b22;

}

body {

  margin: 0;

  font-family: 'Poppins', sans-serif;

  background: var(--bg);

  color: var(--text);

  transition: background 0.5s, color 0.5s;

}

/* Splash Screen with animated SVG */

#splash {

  position: fixed;

  top: 0; left: 0;

  width: 100%; height: 100%;

  background: linear-gradient(135deg, var(--primary), var(--secondary));

  display: flex;

  flex-direction: column;

  justify-content: center;

  align-items: center;

  color: white;

  z-index: 9999;

  animation: fadeOut 2s ease 2.5s forwards;

}

.svg-wrapper { animation: zoom 2s ease infinite alternate; }

.spin-circle { animation: spin 3s linear infinite; }

@keyframes spin {

  from { transform: rotate(0deg); transform-origin: center; }

  to { transform: rotate(360deg); transform-origin: center; }

}

@keyframes zoom {

  from { transform: scale(1); opacity: 1; }

  to { transform: scale(1.1); opacity: 0.9; }

}

@keyframes fadeOut {

  to { opacity: 0; visibility: hidden; }

}

.splash-text { font-size: 2rem; margin: 10px 0 5px; }

.splash-sub { font-size: 1rem; opacity: 0.85; }

.hidden { display: none; }

/* Header */

header {

  display: flex;

  justify-content: space-between;

  align-items: center;

  padding: 15px 30px;

  background: var(--primary);

  color: white;

}

.logo-area { display:flex; align-items:center; gap:10px; }

.logo-text { margin:0; font-size:1.1rem; color:white; }

/* Nav */

nav a { margin: 0 10px; color: white; text-decoration: none; font-weight: 500; }

/* Toggle label simple */

.toggle-label { display: flex; align-items: center; gap: 5px; cursor: pointer; }

/* Dashboard */

.dashboard { padding: 60px 40px; text-align: center; background: linear-gradient(180deg, #f9fbff, #edf4ff); }

.dashboard-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 20px; }

.dash-card { background: var(--card-bg); border-radius: 15px; padding: 20px; box-shadow: 0 3px 10px rgba(0,0,0,0.08); }

.amount { font-size: 2rem; font-weight: bold; color: var(--primary); }

/* Voice & Goals */

.voice-assistant, .smart-goals { padding: 60px 40px; text-align: center; }

.assistant-box { display: flex; justify-content: center; gap: 10px; flex-wrap:wrap; }

#voiceInput, #goalInput { padding: 12px; width: 280px; border-radius: 25px; border: 1px solid #ccc; outline: none; background: var(--card-bg); color: var(--text); }

button { background: var(--primary); color: white; border: none; border-radius: 25px; padding: 10px 25px; cursor: pointer; transition: 0.3s; }

button:hover { background: var(--secondary); }

/* Floating mic */

.float-mic {

  position: fixed;

  bottom: 80px; right: 25px;

  background: var(--secondary); border: none; border-radius: 50%;

  width: 60px; height: 60px; font-size: 1.5rem; color: white;

  box-shadow: 0 4px 10px rgba(0,0,0,0.3); cursor: pointer; transition: transform 0.3s ease; z-index: 99;

}

.float-mic:hover { transform: scale(1.1); }

/* Bottom nav */

.bottom-nav {

  position: fixed; bottom: 0; left: 0; width: 100%;

  background: var(--primary); display:flex; justify-content: space-around; padding: 10px 0; z-index: 100;

}

.bottom-nav button { background: none; border: none; color: white; font-size: 1.4rem; }

/* Language select */

.lang-select { margin: 15px 0; }

.lang-select select { padding: 8px 12px; border-radius: 10px; border: 1px solid #ccc; background: var(--card-bg); color: var(--text); font-size: 1rem; }

/* Footer */

footer { background: var(--primary); color: white; text-align:center; padding: 15px; }

.hidden-screen { display: none; }

/* Responsive */

@media (max-width: 768px) {

  .desktop-nav { display: none; }

  #voiceInput, #goalInput { width: 70%; }

}
// Splash screen loader

window.addEventListener("load", () => {

  setTimeout(() => {

    const splash = document.getElementById("splash");

    if (splash) splash.style.display = "none";

    const app = document.getElementById("app-content");

    if (app) app.classList.remove("hidden");

    speak("Welcome to FinOne, Finance for Everyone, Everywhere.");

  }, 3500);

});

let selectedLang = "en-IN";

// Speak (speech synthesis) with language support

function speak(text) {

  if (!window.speechSynthesis) return;

  const synth = window.speechSynthesis;

  const utter = new SpeechSynthesisUtterance(text);

  utter.lang = selectedLang;

  utter.rate = 1.05;

  synth.speak(utter);

}

// Language selector

const languageSelect = document.getElementById("languageSelect");

if (languageSelect) {

  languageSelect.addEventListener("change", (e) => {

    selectedLang = e.target.value || "en-IN";

    speak(selectedLang === "hi-IN" ? "नमस्ते! मैं FinOne असिस्टेंट हूँ।" : "Hello! I'm FinOne Assistant.");

  });

}

// Speech recognition (browser)

const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;

const recognition = SpeechRecognition ? new SpeechRecognition() : null;

if (recognition) {

  recognition.continuous = false;

  recognition.interimResults = false;

}

// DOM references

const listenBtn = document.getElementById("listenBtn");

const voiceInput = document.getElementById("voiceInput");

const responseBox = document.getElementById("response");

const sendCommandBtn = document.getElementById("sendCommand");

// Start listening (mic) button

if (recognition && listenBtn) {

  listenBtn.addEventListener("click", () => {

    recognition.lang = selectedLang;

    speak(selectedLang === "hi-IN" ? "बोलिए, मैं सुन रहा हूँ।" : "I'm listening...");

    recognition.start();

  });

  recognition.onresult = (event) => {

    const command = event.results[0][0].transcript;

    if (voiceInput) voiceInput.value = command;

    handleCommand(command);

  };

  recognition.onerror = () => {

    speak(selectedLang === "hi-IN" ? "माइक्रोफ़ोन नहीं सुन पा रहा।" : "Microphone error.");

  };

}

// Click Send (typed command)

if (sendCommandBtn) {

  sendCommandBtn.addEventListener("click", () => {

    const cmd = voiceInput ? voiceInput.value : "";

    handleCommand(cmd);

  });

}

// Command processing

function handleCommand(commandText) {

  if (!commandText) return;

  const command = commandText.toLowerCase().trim();

  if (command.includes("send") && command.includes("500")) {

    if (responseBox) responseBox.textContent = "✅ Sending ₹500 to Rahul Kumar...";

    speak(selectedLang === "hi-IN" ? "₹500 राहुल को भेज रहा हूँ।" : "Sending ₹500 to Rahul Kumar.");

  } else if (command.includes("balance")) {

    if (responseBox) responseBox.textContent = "💰 Your balance is ₹4,250.";

    speak(selectedLang === "hi-IN" ? "आपका बैलेंस ₹४,२५० है।" : "Your balance is ₹4,250.");

  } else if (command.includes("goal") || command.includes("save")) {

    if (responseBox) responseBox.textContent = "🎯 Goal recorded: " + command;

    speak(selectedLang === "hi-IN" ? "लक्ष्य सेव किया गया।" : "Goal saved successfully.");

  } else {

    if (responseBox) responseBox.textContent = "🤖 Sorry, I didn’t understand.";

    speak(selectedLang === "hi-IN" ? "माफ़ करें, मैं समझ नहीं पाया।" : "Sorry, I didn’t understand that.");

  }

}

// Smart Goals: save

const saveGoalBtn = document.getElementById("saveGoal");

if (saveGoalBtn) {

  saveGoalBtn.addEventListener("click", () => {

    const goalInput = document.getElementById("goalInput");

    const goalDisplay = document.getElementById("goalDisplay");

    if (!goalInput || !goalDisplay) return;

    const goal = goalInput.value.trim();

    if (!goal) return;

    goalDisplay.textContent = `🎯 Your goal: ${goal}`;

    speak(selectedLang === "hi-IN" ? `आपका लक्ष्य सेव किया गया है: ${goal}` : `Goal saved: ${goal}`);

  });

}

// AI Insights

const askAI = document.getElementById("askAI");

if (askAI) {

  askAI.addEventListener("click", () => {

    const tips = [

      "Your savings increased 15% this week!",

      "Consider investing 10% of your income.",

      "Try setting a micro goal for emergency savings.",

      "Reduce spending on dining by 5% next month.",

      "You're doing great! Keep saving smartly."

    ];

    const randomTip = tips[Math.floor(Math.random() * tips.length)];

    const aiInsight = document.getElementById("aiInsight");

    if (aiInsight) aiInsight.textContent = randomTip;

    speak(selectedLang === "hi-IN" ? "आपकी सेविंग्स 15 प्रतिशत बढ़ी हैं!" : randomTip);

  });

}

// Refresh balance

const refreshBalance = document.getElementById("refreshBalance");

if (refreshBalance) {

  refreshBalance.addEventListener("click", () => {

    const newBal = Math.floor(Math.random() * 5000 + 3000);

    const amountEl = document.querySelector(".amount");

    if (amountEl) amountEl.textContent = `₹${newBal}`;

    speak(selectedLang === "hi-IN" ? `आपका नया बैलेंस है ₹${newBal}` : `Your updated balance is ₹${newBal}`);

  });

}

// Bottom navigation behavior

const navButtons = document.querySelectorAll(".bottom-nav button");

const sections = document.querySelectorAll("main section");

navButtons.forEach(btn => {

  btn.addEventListener("click", () => {

    const t = btn.getAttribute("data-target");

    sections.forEach(s => s.classList.toggle("hidden-screen", s.id !== t));

  });

});

// Floating mic opens assistant

const floatMic = document.getElementById("floatMic");

if (floatMic) {

  floatMic.addEventListener("click", () => {

    sections.forEach(s => s.classList.toggle("hidden-screen", s.id !== "voice"));

    speak(selectedLang === "hi-IN" ? "नमस्ते, मैं आपकी क्या मदद कर सकता हूँ?" : "Hi, how can I help you today?");

  });

}

// Theme toggle

const themeToggle = document.getElementById("themeToggle");

if (themeToggle) {

  themeToggle.addEventListener("change", (e) => {

    document.body.classList.toggle("dark", e.target.checked);

  });

}
