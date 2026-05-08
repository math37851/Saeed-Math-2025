# 🦘 منصة تدريب كانجارو للموهوبين

> **Kangaroo Math Competition Training Platform**  
> An interactive Arabic-language web app for practising Kangaroo math competition questions (Years 2020 – 2025).

---

## ✨ Features

| Feature | Details |
|---|---|
| 📚 Question Bank | 180 questions across 6 years (2020–2025), 30 per year |
| 🏷️ Difficulty Levels | Level 3 (3 pts) · Level 4 (4 pts) · Level 5 (5 pts) |
| 💡 Detailed Feedback | Step-by-step Arabic explanation + solving strategy for every question |
| 🖼️ Visual Questions | Original competition images embedded per question |
| 🌙 Dark / Light Mode | Full theme support |
| 📊 Progress Tracking | Firebase Realtime Database — tracks answers, scores, streaks |
| 📱 Responsive | Mobile-first RTL layout (Arabic, Tajawal font) |

---

## 🗂️ Project Structure

```
Kangaroo_Release_2025/
├── index.html          # Main single-page application
├── data.js             # All 180 questions with answers, explanations & strategies
├── assets/             # Question images  (q_YEAR_NUM.png)
└── q_2023_*.png        # 2023 question images (real paper scans)
```

---

## 🚀 Getting Started

The app is a **static single-page application** — no build step required.

### Run locally

```bash
# Any static file server works, e.g.:
npx serve .
# or
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

### Deploy

Upload the entire `Kangaroo_Release_2025/` folder to any static host (GitHub Pages, Netlify, Firebase Hosting, etc.).

---

## 📦 Data Format (`data.js`)

```js
const QUESTIONS_DATA = [
  {
    year: 2025,
    q_num: 1,
    points: 3,
    correct: "A",
    options: { A: "...", B: "...", C: "...", D: "...", E: "..." },
    explanation: "شرح تفصيلي بالعربية ...",
    strategy: "استراتيجية الحل ..."
  },
  // ...
];
```

---

## 🗓️ Years Covered

| Year | Questions | Status |
|------|-----------|--------|
| 2025 | 30 | ✅ Complete |
| 2024 | 30 | ✅ Complete |
| 2023 | 30 | ✅ Complete |
| 2022 | 30 | ✅ Complete |
| 2021 | 30 | ✅ Complete |
| 2020 | 30 | ✅ Complete |

---

## 🛠️ Tech Stack

- **Frontend**: Vanilla HTML / CSS / JavaScript (RTL Arabic)
- **Font**: [Tajawal](https://fonts.google.com/specimen/Tajawal) via Google Fonts
- **Icons**: Font Awesome 6
- **Database**: Firebase Realtime Database (progress tracking)

---

## 📄 License

For educational use. Competition questions are the property of the Kangaroo Math Association.
