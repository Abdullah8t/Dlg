# CurioCraft Hausa 🧠🇳🇬
### Koyon Shirin Kwamfuta a Harshen Hausa

AI-powered programming education app in Hausa for Python, Java & C++.

---

## ⚡ Quick Setup (5 minutes)

### 1. Install dependencies
```bash
npm install
```

### 2. Add your API Key
Open `src/data/api.js` and replace:
```js
const API_KEY = 'YOUR_ANTHROPIC_API_KEY';
```
with your actual Anthropic API key from https://console.anthropic.com

### 3. Run on Android
```bash
# Option A: Expo Go (fastest — no build needed)
npx expo start
# Then scan QR code with Expo Go app on your phone

# Option B: Direct Android (needs USB debugging)
npx expo start --android
```

---

## 📦 Build APK (for distribution)

### Install EAS CLI
```bash
npm install -g eas-cli
eas login
eas build:configure
```

### Build APK
```bash
# Development APK (sideload)
eas build --platform android --profile preview

# Production AAB (Play Store)
eas build --platform android --profile production
```

---

## 📁 Project Structure
```
curioscraft-hausa/
├── App.js                    # Navigation setup
├── app.json                  # Expo config
├── src/
│   ├── data/
│   │   ├── api.js            # Claude AI API calls
│   │   └── constants.js      # Colors, languages, topics
│   └── screens/
│       ├── HomeScreen.js     # Language selection
│       ├── TopicsScreen.js   # Topic list
│       └── LessonScreen.js   # Full lesson experience
└── assets/                   # Icons & images
```

---

## ✨ Features
- 🇳🇬 Full Hausa language interface
- 🐍☕⚙️ Python, Java, C++ — 8 lessons each
- 📖 AI-generated explanations in Hausa
- 💻 Code examples with Hausa comments
- 🤔 Socratic thinking questions
- 🎯 Interactive quiz with feedback
- 🏆 Progress tracking per lesson
- 📱 Native Android feel

---

## 🔑 Getting an API Key
1. Go to https://console.anthropic.com
2. Sign up / log in
3. Go to "API Keys" → "Create Key"
4. Copy and paste into `src/data/api.js`
