# LeetCode Stepwise Helper - Chrome Extension 

This is a Chrome Extension that helps users get stepwise AI-generated hints while solving LeetCode problems.

---

## Features:

- Extracts LeetCode problem title and user's current code
- Sends them to a deployed AI backend (GROQ API via Render)
- Returns one logical step hint to help users progress without full code solution

---

## How to Install Locally:

1. Clone this repository or download as ZIP and extract.

2. In Chrome:
- Go to `chrome://extensions/`
- Turn ON **Developer Mode**
- Click **Load unpacked**
- Select this project folder.

3. Make sure `popup.js` points to the correct backend API like:

```javascript
fetch('https://leetcode-extension-backend-yj4g.onrender.com/getHint', {...})
