# 🏋️ Gravity Fitness

> **Defy Limits. Own Your Strength.**  
> A modern, high-performance web experience for **Gravity Fitness** — featuring responsive design, dark/light theme toggle, interactive BMI calculator, dynamic testimonials carousel, class schedules, trainer profiles, transparent membership tiers, and a comprehensive primary & alternative contact system.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Contact & Facility Reference](#-contact--facility-reference)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Design System & Theme](#-design-system--theme)
- [Browser Compatibility](#-browser-compatibility)
- [License & Credits](#-license--credits)

---

## 🌟 Overview

**Gravity Fitness** is designed for modern athletes, fitness enthusiasts, and newcomers looking to take their physical conditioning and health to the next level. The website delivers an engaging digital storefront with fast load times, accessible semantic HTML5 markup, smooth scrolling navigation, and full mobile optimization.

---

## ⚡ Key Features

- **Responsive Multi-Device Layout**: Fluid experience optimized across mobile phones, tablets, laptops, and ultra-wide desktop monitors.
- **Dark Mode / Light Mode Switcher**:
  - One-click toggle button with dynamic sun/moon icons.
  - Automatically respects user OS system preference (`prefers-color-scheme`).
  - Persists state across browser sessions via `localStorage`.
- **Primary & Alternative Contact Integration**:
  - Quick action contact cards for phone, email, multi-facility locations, and WhatsApp.
  - Dedicated interactive contact & consultation form with instant visual confirmation.
  - One-tap `tel:` and `mailto:` direct links.
- **Interactive BMI Calculator**:
  - Live metric calculator (height in cm, weight in kg).
  - Form validation with descriptive error guidance.
  - Instant classification output (Underweight, Healthy Weight, Overweight, Obese) with visual color accents.
- **Featured Fitness Classes**:
  - Grid presentation of core training disciplines: *Body Building*, *Power Lifting*, *Cycling*, *Karate*, *Boxing*, and *Conditioning*.
  - Displays dedicated coaches and class schedules.
- **Trainer Profiles**:
  - Highlights expert fitness coaches with specialty certifications and social channel links.
- **Testimonial Slider**:
  - Automatic 5-second interval rotating testimonial showcase with manual selector controls.
- **Transparent Membership Pricing**:
  - Three distinct membership plans (*Basic*, *Pro*, and *Elite*) with detailed feature breakdowns and direct signup links.
- **Video & Media Showcase**:
  - Interactive training video playback with custom overlay play/pause toggling.
- **Material Ripple Interaction**:
  - Custom ripple effects on all buttons and interactive anchor elements.

---

## 📞 Contact & Facility Reference

Gravity Fitness maintains both primary channels and alternative support routes to ensure immediate assistance for members and visitors:

| Channel / Service | Primary Details | Alternative Details | Hours / Availability |
| :--- | :--- | :--- | :--- |
| **Phone Line** | `+1 (800) 472-8489`<br>*(1-800-GRAVITY)* | `+1 (212) 555-0198`<br>*(Direct Desk)* | Mon – Fri: 6:00 AM – 10:00 PM<br>Sat – Sun: 7:00 AM – 9:00 PM |
| **Email Inquiries** | [`contact@gravityfitness.com`](mailto:contact@gravityfitness.com) | [`support@gravityfitness.com`](mailto:support@gravityfitness.com) | 2-Hour Response Time Guarantee |
| **Locations** | **Downtown Flagship HQ**<br>742 Evergreen Terrace, Suite 300<br>New York, NY 10001 | **West Campus Training Annex**<br>180 Olympic Boulevard<br>Brooklyn, NY 11201 | Open 7 Days a Week |
| **Instant Messaging** | **WhatsApp Desk**: [`+1 (212) 555-0199`](https://wa.me/12125550199) | **24/7 Member Crisis Desk** | 24 Hours / 7 Days a Week |

### Facility Operating Hours

- **Monday – Thursday**: `6:00 AM – 10:00 PM`
- **Friday**: `6:00 AM – 11:00 PM`
- **Saturday**: `7:00 AM – 9:00 PM`
- **Sunday**: `7:00 AM – 9:00 PM`

---

## 💻 Tech Stack

- **Markup**: HTML5 with semantic structure and descriptive ARIA labels
- **Styling**: Tailwind CSS utility framework supplemented by custom CSS variables (`src/input.css`)
- **Icons**: Font Awesome 6 Free (Solid, Regular, Brands)
- **Typography**: Google Fonts (*Roboto*, sans-serif)
- **Interactivity**: Vanilla JavaScript (ES6+) for theme toggling, BMI logic, sliders, and navigation handlers

---

## 📁 Project Structure

```text
Gravity-Fitness/
├── content/                     # Images, illustrations, and media assets
│   ├── bg1.webp                 # Testimonials background
│   ├── bg2.webp                 # BMI calculator background
│   ├── classes1.webp..classes8  # Featured class photography
│   ├── landing.webp             # Hero section background
│   ├── man1.webp..man5.webp     # Trainer and member photos
│   ├── pic1.webp..pic6.jpeg     # Features and pricing card imagery
│   └── video1.mp4               # Promotional facility clip
├── dist/
│   └── output.css               # Compiled Tailwind utility classes
├── src/
│   ├── all.min.css              # Font Awesome stylesheet
│   ├── classes.js               # Class page utilities & theme persistence
│   ├── input.css                # Base stylesheet, CSS variables, & custom components
│   └── main.js                  # Core application logic (theme, BMI, slider, form)
├── webfonts/                    # Font Awesome binary webfont files (woff2/ttf)
├── index.html                   # Main single-page web application
├── package.json                 # Project configuration and metadata
├── package-lock.json            # Dependency tree lockfile
├── tailwind.config.js           # Tailwind theme configuration & custom color tokens
└── README.md                    # Project documentation
```

---

## 🚀 Getting Started

No build step is required to run and test the website! You can view it immediately using any standard web browser or local static server.

### Option 1: Direct File Preview
Simply double-click `index.html` or open it with your preferred browser (Google Chrome, Firefox, Microsoft Edge, Safari).

### Option 2: Local HTTP Server (Recommended)
Using Node.js:
```bash
# Using npx serve
npx serve .
```

Or using Python:
```bash
# Python 3
python -m http.server 3000
```
Open your browser and navigate to `http://localhost:3000`.

### Option 3: VS Code Live Server
1. Install the **Live Server** extension in VS Code.
2. Right-click `index.html` and select **"Open with Live Server"**.

---

## 🎨 Design System & Theme

The project uses HSL/RGB custom properties for consistent theming and dark mode inversion:

| Token | Light Mode Value | Dark Mode Value | Usage |
| :--- | :--- | :--- | :--- |
| `--color-primary` | `182 36 79` (`#b6244f`) | `182 36 79` (`#b6244f`) | Brand crimson highlight & action buttons |
| `--bgc1` | `255 255 255` | `40 40 40` | Primary surface background |
| `--bgc2` | `235 235 235` | `30 30 30` | Secondary surface cards & footer |
| `--text1` | `40 40 40` | `255 255 255` | Primary body and heading typography |
| `--text4` | `125 125 125` | `255 255 255` | Secondary text & subtitles |

---

## 🌐 Browser Compatibility

Tested and fully functional on:
- Google Chrome (latest)
- Mozilla Firefox (latest)
- Microsoft Edge (latest)
- Apple Safari (iOS & macOS)
- Opera (latest)

---

## 📄 License & Credits

- **Brand**: Gravity Fitness &copy; 2026. All rights reserved.
- **Icons**: [Font Awesome](https://fontawesome.com/)
- **Fonts**: [Google Fonts (Roboto)](https://fonts.google.com/specimen/Roboto)
