# 🏥 SmartTriage & Clinic Navigator

[![Live Demo](https://img.shields.io/badge/demo-live-success)](https://Shlokyadav-0315.github.io/SmartTriage)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

> **A modern, AI-powered healthcare triage application that helps patients assess their symptoms and find appropriate care facilities nearby.**

## 🌐 Live Demo

**👉 [Try SmartTriage Now](https://Shlokyadav-0315.github.io/SmartTriage) 👈**

Simply open the link above to start using the application immediately - no installation required!

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Screenshots](#screenshots)
- [How It Works](#how-it-works)
- [Technology Stack](#technology-stack)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## 🎯 Overview

**SmartTriage** addresses the critical problem of post-pandemic healthcare facility intake bottlenecks. Non-emergency patients often overwhelm ERs or struggle to communicate their medical history effectively. Our solution provides:

- **AI-Assisted Triage**: Intelligent urgency level assessment (Low/Moderate/Emergency)
- **Facility Locator**: Find nearby healthcare centers based on your urgency level
- **Medical Summary**: Download a professional 1-page intake summary for your doctor
- **Bilingual Support**: Available in English and Hindi (हिन्दी)

---

## ✨ Features

### 🎨 Modern UI/UX
- Beautiful gradient-based design with glass-morphism effects
- Smooth animations and transitions
- Fully responsive (mobile, tablet, desktop)
- Interactive symptom selection cards
- Real-time progress tracking

### 🤖 Smart Triage System
- AI-powered urgency classification
- Three-tier assessment (Low, Moderate, Emergency)
- Comprehensive symptom analysis
- Pain level tracking (0-10 scale)
- Critical symptom detection

### 📍 Facility Finder
- Location-based healthcare facility search
- GPS integration for automatic location
- Facilities filtered by urgency level
- Distance, wait times, and contact information
- One-click directions

### 📄 Medical Intake Summary
- Professional PDF generation
- Complete patient information
- Detailed symptom description
- AI triage assessment results
- Care recommendations

### 🌍 Bilingual Support
- **English** and **Hindi (हिन्दी)** interface
- Real-time language switching
- Comprehensive translations (100+ phrases)
- No page reload required

### ♿ Accessibility
- WCAG-compliant design
- Keyboard navigation support
- Screen reader friendly
- High contrast ratios

---

## 📸 Screenshots

### Welcome Screen
Beautiful landing page with feature highlights and call-to-action.

### Symptom Assessment
Interactive symptom cards with visual feedback and comprehensive input options.

### Triage Results
Color-coded urgency levels with personalized recommendations and emergency warnings.

### Facility Locator
Map view with nearby healthcare facilities, ratings, and contact information.

---

## 🔄 How It Works

### Step 1: Basic Information
Enter your personal details, medical history, known allergies, and current medications.

### Step 2: Symptom Assessment
- Select your primary symptom category
- Describe symptoms in detail
- Indicate when symptoms started
- Rate pain level (if applicable)
- Check for critical symptoms

### Step 3: AI Triage Assessment
Receive your urgency level:
- **🟢 LOW**: Routine care appropriate - schedule a regular appointment
- **🟡 MODERATE**: Prompt care recommended - visit clinic within 24 hours
- **🔴 EMERGENCY**: Immediate care required - call 108/102 or go to ER

### Step 4: Find Care & Download
- Search for nearby healthcare facilities
- Get personalized facility recommendations
- Download your medical intake summary (PDF)
- Navigate to your chosen facility

---

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: TailwindCSS (CDN)
- **PDF Generation**: jsPDF
- **Icons & Graphics**: SVG, Custom Logo Design
- **Fonts**: Google Fonts (Poppins)
- **Architecture**: Single Page Application (SPA)
- **Deployment**: GitHub Pages

**No backend required!** The application runs entirely in the browser.

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection (for CDN resources)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Shlokyadav-0315/SmartTriage.git
cd SmartTriage
```

2. **Open the application**
```bash
# Simply open index.html in your browser
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

Or use a local server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve

# Using PHP
php -S localhost:8000
```

3. **Visit** `http://localhost:8000`

---

## 📖 Usage

### For Patients

1. **Access the App**: Open the [live demo](https://Shlokyadav-0315.github.io/SmartTriage) or run locally
2. **Start Assessment**: Click "Start Your Assessment"
3. **Fill Information**: Complete all four steps
4. **Get Results**: Review your triage level and recommendations
5. **Find Care**: Search for nearby facilities
6. **Download Summary**: Get your PDF to bring to the doctor

### For Developers

**Customize Triage Logic**:
```javascript
// Located in the performTriage() function
// Modify scoring algorithm around line 1040
if (patientData.difficultBreathing) {
    score += 30; // Adjust weight
}
```

**Add New Facilities**:
```javascript
// Located in generateFacilities() function
// Add your local healthcare facilities around line 1190
```

**Customize Translations**:
```javascript
// Located in translations object around line 880
const translations = {
    en: { /* English translations */ },
    hi: { /* Hindi translations */ }
};
```

---

## 📁 Project Structure

```
SmartTriage/
│
├── index.html              # Main application file
├── translations.js         # Separate translation dictionary (optional)
├── README.md              # This file
├── LICENSE                # MIT License
│
└── assets/                # (Optional) Additional resources
    ├── screenshots/       # Application screenshots
    └── demo/             # Demo videos or GIFs
```

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/AmazingFeature`
3. **Commit your changes**: `git commit -m 'Add some AmazingFeature'`
4. **Push to the branch**: `git push origin feature/AmazingFeature`
5. **Open a Pull Request**

### Contribution Ideas
- Add more languages (Tamil, Telugu, Bengali, etc.)
- Integrate real healthcare facility APIs
- Add symptom search/autocomplete
- Implement appointment booking
- Add medical history storage
- Create mobile app version (React Native/Flutter)

---

## ⚠️ Disclaimer

**IMPORTANT**: SmartTriage is an AI-assisted assessment tool and **should NOT replace professional medical advice, diagnosis, or treatment**. 

- Always seek the advice of qualified healthcare providers
- In case of emergency, call **108 (Emergency)** or **102 (Ambulance)** immediately
- Do not rely solely on this application for medical decisions

This application is designed for educational and informational purposes to help guide patients to appropriate care levels.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Design Inspiration**: Modern healthcare apps and UI/UX best practices
- **Icons**: Material Design Icons, SVG custom designs
- **Fonts**: Google Fonts (Poppins)
- **Libraries**: TailwindCSS, jsPDF
- **Healthcare Data**: Sample facility data for demonstration purposes

--

## 📞 Contact & Support

- **Issues**: [GitHub Issues](https://github.com/Shlokyadav-0315/SmartTriage/issues)
- **Discussions**: [GitHub Discussions](https://github.com/Shlokyadav-0315/SmartTriage/discussions)

---

## 🌟 Star History

If you find this project useful, please consider giving it a star ⭐

[![Star History Chart](https://api.star-history.com/svg?repos=Shlokyadav-0315/SmartTriage&type=Date)](https://star-history.com/Shlokyadav-0315/SmartTriage&Date)

---

## 🔮 Future Roadmap

- [ ] Integration with real healthcare APIs (Google Maps, hospital databases)
- [ ] User accounts and medical history storage
- [ ] Telemedicine integration
- [ ] Appointment scheduling system
- [ ] Medicine reminder feature
- [ ] Health records management
- [ ] Multi-platform mobile apps
- [ ] Voice input for accessibility
- [ ] Offline mode with PWA
- [ ] Insurance integration

---

**Made with ❤️ for better healthcare accessibility**

**#HealthTech #AI #OpenSource #Healthcare #Triage**
