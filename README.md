# 🛡️ SHEild AI — Intelligent Women's Safety Platform

**SHEild AI** is a modern, mobile-first web application designed as a personal safety companion for women. It provides instant emergency tools, real-time location tracking, evidence recording, and one-tap communication with emergency contacts — all without any backend or server required.

> **Built with:** HTML5 · CSS3 · Vanilla JavaScript · Web APIs (Geolocation, MediaRecorder, Speech Recognition)

---

## ✨ Features

### 🚨 Emergency Response
- **SOS Button** — One-tap emergency activation with real-time GPS, evidence recording, and automatic alerts to all saved contacts via WhatsApp & SMS
- **Voice Activation** — Say your custom emergency keyword to trigger SOS hands-free (Web Speech API)
- **Shake-to-Alert** — Shake your phone to instantly activate emergency mode (DeviceMotion API)
- **Fake Call** — Simulate an incoming call to escape uncomfortable situations

### 📍 Live Location Tracking
- Real-time GPS tracking with embedded Google Maps
- Live coordinates display (latitude, longitude, accuracy)
- Share location instantly via **WhatsApp**, **SMS**, **clipboard**, or native share
- Duration timer for tracking sessions

### 💬 Emergency Chat
- Chat-like interface to message emergency contacts
- Send messages via **WhatsApp** or **SMS** with one tap
- Quick reply buttons: *"Send Help"*, *"I'm Safe"*, *"Track Me"*, *"Call Me"*
- **Attach GPS location** to any message
- **Record & share audio** evidence directly from chat

### 📞 Helplines
- Dedicated page with India's emergency helpline numbers
- **One-tap call** buttons using `tel:` links
- Categories: Emergency, Women's Safety, Other Support
- Includes: Women Helpline (181), Police (100), Universal Emergency (112), Domestic Violence (1091), Childline (1098), Cyber Crime (1930), and more

### 🎤 Evidence Recording
- **Video + Audio** recording during emergencies (camera + mic)
- **Audio-only** fallback when camera is unavailable
- Standalone audio evidence recording from dashboard
- All evidence files saved as downloadable `.webm` files

### 🔊 Siren Alarm
- Loud siren sound via Web Audio API
- Auto-stops after 10 seconds

### 🗣️ Audio Guide
- Voice-guided instructions using Web Speech Synthesis
- Helps users who can't read the interface

### 🛡️ Safety Score
- Measures your safety readiness (profile, contacts, PIN, keyword)
- Visual progress bars for each category

### 📁 Incident Vault
- View all past emergency incidents
- Filter by today, this week, or all time
- Download incident reports as `.txt` files

### ⚙️ Settings
- Update emergency keyword and security PIN
- Toggle voice activation
- Light/Dark theme switching
- Reset all data

---

## 📁 Project Structure

```
sheild-ai/
├── index.html            # Landing page
├── onboarding.html       # First-time setup (keyword, PIN)
├── dashboard.html        # Main safety dashboard
├── emergency.html        # Emergency mode (recording, GPS, alerts)
├── contacts.html         # Manage emergency contacts (up to 5)
├── livelocation.html     # Live GPS tracking & sharing
├── chat.html             # Emergency chat with contacts
├── helplines.html        # Emergency helpline numbers
├── safezones.html        # Find nearby safe areas
├── vault.html            # Incident history & reports
├── settings.html         # App settings
├── css/
│   └── style.css         # Complete design system & styles
└── js/
    └── script.js         # All application logic
```

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome recommended for voice features)
- No Node.js, npm, or backend required

### Run Locally

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/sheild-ai.git
cd sheild-ai

# Option 1: Open directly
# Just open index.html in your browser

# Option 2: Local server (for GPS/camera access)
python -m http.server 8080
# Then open http://localhost:8080
```

> **Note:** GPS and camera features require HTTPS in production. For local development, `localhost` works fine.

### Deploy to GitHub Pages

1. Push your code to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch** → `main` → `/ (root)`
4. Your app will be live at `https://YOUR_USERNAME.github.io/sheild-ai/`

---

## 📱 How It Works

1. **Onboarding** — Set your emergency keyword and security PIN
2. **Add Contacts** — Save up to 5 trusted emergency contacts
3. **Dashboard** — Access all safety features from one place
4. **SOS** — Tap the SOS button or say your keyword to activate emergency mode
5. **Emergency Mode** — Automatically records evidence, tracks GPS, and alerts all contacts via WhatsApp & SMS
6. **Stop Emergency** — Enter your PIN to deactivate and save all evidence

---

## 🔒 Privacy

- **100% client-side** — No data is sent to any server
- All data is stored in `localStorage` on your device
- Evidence files are saved to your device's Downloads folder
- GPS coordinates are only shared when you explicitly trigger SOS or share location

---

## 🛠️ Technologies Used

| Technology | Usage |
|-----------|-------|
| HTML5 | Semantic structure |
| CSS3 | Glassmorphism, animations, responsive design |
| Vanilla JavaScript | All application logic |
| Geolocation API | Real-time GPS tracking |
| MediaRecorder API | Audio/video evidence recording |
| Web Speech API | Voice recognition & audio guide |
| Web Audio API | Siren alarm |
| Web Share API | Native sharing on mobile |

---

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<p align="center">
  Made with ❤️ for women's safety
</p>
