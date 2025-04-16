# 🛡️ Phishing Attack Saver – Chrome Extension 🔐

Protect yourself from phishing attempts in real-time using this smart Chrome Extension that detects and blocks suspicious websites through client-side heuristics. No need for server-side lookups — lightweight, fast, and privacy-focused!

## 🚀 Overview

**Phishing Attack Saver** is a Chrome Extension designed to guard users against phishing websites by applying local heuristic analysis directly in the browser. It analyzes page content, URLs, and DOM behavior to detect common signs of phishing attacks, warning users before they fall victim.

## 🔍 Features

- ✅ **Client-Side Heuristics Detection**: Analyzes page elements, link mismatches, suspicious form actions, and more without needing a remote server.
- 🌐 **Real-Time Protection**: Monitors browsing activity and immediately alerts users when a potential phishing page is detected.
- 🧠 **Intelligent Heuristics Engine**: Uses multiple criteria like URL patterns, iframe usage, keyword detection, and domain reputation.
- 🔔 **User Alerts**: Pop-up warnings for suspicious sites with options to proceed or go back safely.
- 🧩 **Lightweight and Secure**: Fully self-contained — no data leaves your browser!

## 🛠️ Technologies Used

- Manifest V3
- JavaScript (Vanilla)
- Chrome Extension APIs (tabs, runtime, scripting)
- DOM Analysis Techniques
- Optional integration-ready with Google Safe Browsing or other APIs

## 🗂️ Project Structure

```
phishing-attack-saver-extension/
├── background.js              # Background script for tab monitoring
├── content.js                 # Injected into pages to run heuristics
├── popup.html                 # Popup UI
├── popup.js                   # Logic for popup actions
├── manifest.json              # Chrome extension manifest (V3)
├── icons/                     # Extension icons
└── heuristics.js              # Core heuristics engine
```

## ⚙️ Installation (Developer Mode)

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/phishing-attack-saver-extension.git
   ```

2. Open Chrome and go to:
   ```
   chrome://extensions/
   ```

3. Enable **Developer Mode** (top right).

4. Click **Load unpacked** and select the cloned project folder.

5. You’re good to go! The extension will now analyze websites as you browse.

## 📈 Detection Heuristics

This extension checks for:

- Mismatched hyperlink text vs href
- Use of deceptive domain names
- Suspicious form submission targets
- Hidden inputs and unexpected redirects
- Overuse of obfuscated JavaScript or base64 strings
- Known phishing keywords (e.g., "verify your account", "password reset")

## 📦 Future Enhancements

- 🔄 Cloud sync of user-reported phishing domains
- 🤖 Machine learning model integration for better accuracy
- 🌍 Internationalized content support
- 🛡️ Support for Firefox (WebExtension API)

## 🧑‍💻 Contributing

Pull requests are welcome! Please fork the repository and open a PR with clear documentation of any feature or fix. For major changes, please open an issue first.

## 📄 License

MIT License – Feel free to use, modify, and distribute.

## 🙌 Acknowledgements

Inspired by the growing need for client-side, privacy-friendly phishing defense tools. Built with ❤️ by developers for users who care about security.
