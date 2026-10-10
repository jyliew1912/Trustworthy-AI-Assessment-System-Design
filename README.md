# Trustworthy AI (TAI) Assessment System — Frontend

[![Next.js](https://img.shields.io/badge/Next.js-15-black?logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind](https://img.shields.io/badge/Tailwind-CSS-38bdf8?logo=tailwindcss)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> **Portfolio Note**  
> This is my personal portfolio fork of the TAI Lab team project.  

An interdisciplinary platform that audits and visualizes machine learning system trustworthiness across **11 core TAI dimensions**. Built in collaboration with Law and Political Science experts.


## 👩‍💻 My Contributions

I owned the core evaluation experience:

- **Home Dashboard** — Project management console
- **Multi-stage Questionnaire Pipeline** (`/questionnaire`) — Dynamic forms with validation, draft saving, and structured payloads
- **Evaluation Report + Radar Charts** (`/report`) — Chart.js visualization of the 11 TAI dimensions + diagnostic insights
- Optimized **Login** and **TAI-sort** (drag-and-drop indicator prioritization)
- Component testing for the above flows


## 🎬 Demo & Documentation

| 📺 Video Demonstration | 📑 Technical Presentation |
| :--- | :--- |
| [![Watch Demo](https://img.youtube.com/vi/jxtBbBmE0rw/hqdefault.jpg)](https://www.youtube.com/watch?v=jxtBbBmE0rw) | [![View PDF](https://img.shields.io/badge/View_Presentation-PDF-red?style=for-the-badge&logo=adobe-acrobat-reader)](docs/FinalProjectPresentation.pdf) |
| End-to-end audit flow: prioritization → questionnaire → radar report | Architecture, governance framework, and scoring design |


## 🌟 System Overview

```text
[ Auditor ]
     │
     ▼
[ Next.js 15 Web Portal ]          ←── This repository (my main work)
  ├── Multilingual App Router (EN / ZH-TW)
  ├── Drag-and-Drop Prioritization (`/tai_sort`)
  ├── Tri-Stage Questionnaire (Pre / Mid / Post)
  └── Dynamic Radar Chart Report Engine
     │
     ▼  REST API
[ TAI Backend Scoring Engine ]
```

**11 TAI Pillars:** Accuracy • Reliability • Safety • Resilience • Transparency • Accountability • Explainability • Autonomy • Privacy • Fairness • Security


## 🛠️ Tech Stack

- **Framework**: Next.js 15 (App Router)
- **Language**: TypeScript 5
- **UI**: Tailwind CSS, Lucide React
- **Charts**: Chart.js + react-chartjs-2
- **i18n**: react-i18next (English + Traditional Chinese)

## ⚡ Getting Started

```bash
git clone https://github.com/jyliew1912/Trustworthy-AI-Assessment-System-Design.git
cd Trustworthy-AI-Assessment-System-Design
npm install

# Create .env.local
echo "NEXT_PUBLIC_API_BASE_URL=http://localhost:3001" > .env.local

npm run dev
```

Open http://localhost:3000  
(Requires the TAI Backend running on port 3001)


## 👥 Engineering Team

| Member | Focus Area |
|--------|------------|
| **劉靖媛 ([@jyliew1912](https://github.com/jyliew1912))** | • Engineered Home dashboard, Report page, and multi-stage Questionnaire flows with component testing<br>• Optimized Login and TAI-sort indicator prioritization interfaces |
| 呂辰祐 (@Shangguanmoxi520) | • Implemented Response History log (`/history`) and Pre-login onboarding landing views<br>• Built structured evaluation Response Viewer components |
| 王峻文 (@codingkcc) | • Developed Admin dashboard (`/admin`) and About page documentation<br>• Integrated multilingual translation pipeline (i18n) and drafted initial TAI-sort module |
| Max Drechsler (@MaxDrechsler) | • Developed initial Login workflow architecture<br>• Coordinated frontend development standards and established unit testing infrastructure |

## 📄 License

MIT License. See [LICENSE](LICENSE).

**Original team repository:** [TAI-trustworthy-ai-lab/Trustworthy-AI-Assessment-System-Design](https://github.com/TAI-trustworthy-ai-lab/Trustworthy-AI-Assessment-System-Design)