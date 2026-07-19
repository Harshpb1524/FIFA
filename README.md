# ⚽ StadiumAI — FIFA World Cup 2026 Intelligence Platform

![StadiumAI Banner](https://img.shields.io/badge/FIFA_WC_2026-StadiumAI-gold?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHRleHQgeT0iMjAiIGZvbnQtc2l6ZT0iMjAiPuKavTwvdGV4dD48L3N2Zz4=)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)
![AI Powered](https://img.shields.io/badge/Powered_by-Gemini_AI-4285F4?style=for-the-badge&logo=google)
![Status](https://img.shields.io/badge/status-Live-brightgreen?style=for-the-badge)

> 🏟️ **A GenAI-powered platform that enhances stadium operations and the overall tournament experience for fans, organizers, volunteers, and venue staff at the FIFA World Cup 2026™.**

---

## 🌟 Overview

**StadiumAI** leverages **Google's Gemini AI** to deliver an intelligent, multilingual, and accessible stadium operations platform for the FIFA World Cup 2026. The platform provides real-time decision support across all 16 venues in the United States, Mexico, and Canada.

### Built for the Google for Developers PromptWar Hackathon

This project demonstrates the transformative potential of Generative AI in enhancing live sporting events at an unprecedented scale — the largest FIFA World Cup in history.

---

## 🚀 Key Features

### 🤖 AI-Powered Smart Assistant
- **Multilingual support** in 9+ languages (English, Spanish, French, Arabic, Portuguese, Japanese, Korean, German, Mandarin)
- Context-aware responses about venues, schedules, navigation, and safety
- Natural conversation interface with markdown rendering
- Personalized recommendations based on user context

### 🗺️ Intelligent Stadium Navigator
- **Interactive SVG stadium maps** with zone-level detail
- AI-generated step-by-step wayfinding directions
- **Accessibility-first routing** (wheelchair accessible, avoid stairs, avoid crowds)
- Real-time POI discovery (food, restrooms, first aid, info desks)

### 👥 Real-Time Crowd Intelligence
- **Live crowd density heatmaps** with zone-by-zone monitoring
- AI-powered crowd flow predictions and peak time alerts
- Entry rate tracking with trend analysis
- Automated crowd management recommendations

### 🚌 Smart Transportation Hub
- Multi-modal route planning (driving, transit, rideshare, walking)
- Real-time parking availability across all lots
- **CO₂ emissions comparison** across transport modes
- Rideshare surge pricing indicators
- AI-optimized route suggestions

### 🌱 Sustainability Dashboard
- **Personal carbon footprint tracker** with eco-score
- Real-time sustainability metrics (waste diversion, water savings, green energy)
- AI-generated eco-tips personalized to user behavior
- Live sustainability feed showing community eco-actions
- Green initiatives showcase for FIFA WC 2026

### ⚙️ Operations Command Center
- **Real-time KPI dashboard** for staff and organizers
- AI-assisted incident management with severity classification
- Automated response recommendations for operational events
- Staff deployment overview and communication tools
- Alert management with priority-based notifications

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────┐
│                   StadiumAI Frontend                 │
│   ┌───────────┬──────────┬──────────┬────────────┐  │
│   │   Home    │    AI    │Navigator │   Crowd    │  │
│   │ Dashboard │Assistant │  & Maps  │   Intel    │  │
│   ├───────────┼──────────┼──────────┼────────────┤  │
│   │ Transport │  Sustain │  Ops     │  Settings  │  │
│   │   Hub     │  ability │ Center   │  & A11y    │  │
│   └───────────┴──────────┴──────────┴────────────┘  │
│                        │                             │
│              ┌─────────▼──────────┐                  │
│              │  Gemini AI Engine  │                  │
│              │  (gemini-2.0-flash)│                  │
│              └─────────┬──────────┘                  │
│                        │                             │
│              ┌─────────▼──────────┐                  │
│              │  Google AI Studio  │                  │
│              │    REST API        │                  │
│              └────────────────────┘                  │
└─────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Semantic structure with accessibility (ARIA) |
| **CSS3** | Custom design system, animations, glassmorphism |
| **Vanilla JavaScript** | Application logic, SPA routing, API integration |
| **Google Gemini AI** | Generative AI for assistant, recommendations, insights |
| **Font Awesome 6** | Iconography |
| **Google Fonts** | Inter & Outfit typography |

### No Build Tools Required
This is a **zero-dependency**, static web application. No npm, no bundlers, no frameworks — just clean, modern web standards. Deploy anywhere that serves static files.

---

## 📦 Getting Started

### Prerequisites
- A modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- A **Google Gemini API Key** ([Get one free from Google AI Studio](https://aistudio.google.com/apikey))

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/fifa-wc2026-stadiumai.git
   cd fifa-wc2026-stadiumai
   ```

2. **Open in browser**
   ```bash
   # Simply open index.html in your browser
   # Or use any static file server:
   npx serve .
   # Or Python:
   python -m http.server 8000
   ```

3. **Configure AI**
   - Click on "AI Assistant" in the sidebar
   - Enter your Gemini API key
   - Start chatting!

### Deploy to GitHub Pages

1. Push the code to your GitHub repository
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch** → **main** → **/ (root)**
4. Your site will be live at `https://YOUR_USERNAME.github.io/fifa-wc2026-stadiumai/`

---

## 🎯 GenAI Integration Details

### How Gemini AI Powers StadiumAI

| Feature | AI Application |
|---|---|
| **Smart Assistant** | Natural language Q&A about all aspects of the World Cup experience |
| **Navigation** | AI-generated step-by-step directions with accessibility considerations |
| **Crowd Management** | AI analysis of crowd patterns with predictive recommendations |
| **Transportation** | AI-optimized route suggestions with environmental impact analysis |
| **Sustainability** | Personalized eco-tips and carbon footprint reduction strategies |
| **Operations** | AI-assisted incident classification and response recommendations |
| **Multilingual** | Automatic language detection and response in 9+ languages |

### API Usage

The application uses the **Gemini 2.0 Flash** model via the REST API:
```
POST https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent
```

**Privacy**: Your API key is stored only in your browser's localStorage and is never transmitted to any server other than Google's AI API.

---

## ♿ Accessibility

StadiumAI is built with accessibility as a core principle:

- ✅ Semantic HTML5 with ARIA labels
- ✅ Keyboard navigation support
- ✅ Screen reader compatible
- ✅ High contrast mode toggle
- ✅ Large text mode
- ✅ Reduced motion support (`prefers-reduced-motion`)
- ✅ Wheelchair-accessible navigation routing
- ✅ Color-blind friendly indicators (shapes + colors)

---

## 🌍 Supported Languages

| Language | Code | Status |
|---|---|---|
| 🇬🇧 English | en | ✅ Full |
| 🇪🇸 Spanish | es | ✅ Full |
| 🇫🇷 French | fr | ✅ Full |
| 🇸🇦 Arabic | ar | ✅ Full |
| 🇧🇷 Portuguese | pt | ✅ Full |
| 🇯🇵 Japanese | ja | ✅ Full |
| 🇰🇷 Korean | ko | ✅ Full |
| 🇩🇪 German | de | ✅ Full |
| 🇨🇳 Mandarin | zh | ✅ Full |

---

## 📁 Project Structure

```
fifa-wc2026-stadiumai/
├── index.html          # Main application HTML
├── css/
│   └── styles.css      # Complete design system & styles
├── js/
│   └── app.js          # Application logic & Gemini integration
├── README.md           # This file
└── LICENSE             # MIT License
```

---

## 🏟️ Supported Venues

The platform covers all **16 FIFA World Cup 2026 venues**:

### 🇺🇸 United States (11 venues)
- MetLife Stadium — East Rutherford, NJ *(Final)*
- SoFi Stadium — Inglewood, CA
- AT&T Stadium — Arlington, TX
- Hard Rock Stadium — Miami Gardens, FL
- NRG Stadium — Houston, TX
- Mercedes-Benz Stadium — Atlanta, GA
- Lincoln Financial Field — Philadelphia, PA
- Gillette Stadium — Foxborough, MA
- Levi's Stadium — Santa Clara, CA
- Arrowhead Stadium — Kansas City, MO
- Lumen Field — Seattle, WA

### 🇲🇽 Mexico (3 venues)
- Estadio Azteca — Mexico City
- Estadio BBVA — Monterrey
- Estadio Akron — Guadalajara

### 🇨🇦 Canada (2 venues)
- BMO Field — Toronto
- BC Place — Vancouver

---

## 🤝 Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Google for Developers** — PromptWar Hackathon
- **Google Gemini AI** — Powering the intelligent features
- **FIFA** — World Cup 2026 inspiration
- **Font Awesome** — Icon library
- **Google Fonts** — Typography (Inter, Outfit)

---

<p align="center">
  <strong>⚽ Built with ❤️ for the FIFA World Cup 2026™ ⚽</strong><br>
  <em>Powered by Google Gemini AI</em>
</p>
