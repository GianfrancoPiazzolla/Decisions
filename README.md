# 🤔 ?ecisions — Schulich Decision Method

![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square)
![PWA](https://img.shields.io/badge/PWA-ready-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-orange?style=flat-square)
![Offline](https://img.shields.io/badge/offline-supported-success?style=flat-square)
![No dependencies](https://img.shields.io/badge/backend-none-lightgrey?style=flat-square)

> **⚖️ A premium, mobile-friendly web app that implements Seymour Schulich's 2:1 decision strategy from *Get Smarter: Life and Business Lessons*.**

---

## ✨ Features

- ✅ **Dual-column scoring** — list positives 👍 on one sheet and negatives 👎 on another
- 🔢 **Score each factor 0–10** with inline editable inputs
- 📊 **Real-time bar chart** comparing positives vs negatives vs the 2× threshold
- 🎯 **Analog gauge** with three verdict zones (🔴 Don't Do It / 🟡 Think Twice / 🟢 Do It)
- 📱 **Mobile-first responsive design** with swipe gestures 👈👉 between tabs
- 🌙 **Dark/Light theme** toggle
- 💾 **Persistent local storage** — with 📥 import and 📤 export features
- 📜 **Decision history** with quick-select and verdict badges
- ❓ **Stylized question‑mark logo** representing life's big choices

---

## 📐 The Schulich Method

Seymour Schulich's decision strategy, described in his book **"Get Smarter: Life and Business Lessons"**, is a simple yet powerful framework for making any important decision. It works in three steps:

### 🧾 Step 1 — List the Positives

Take a sheet of paper and write down **all the positive things** you can think of about the issue in question. For each item, assign a **score from 0 to 10** — the higher the score, the more important that positive factor is to you.

```
Example: "Should I accept this job offer?"
  + Higher salary          → score 9
  + Shorter commute        → score 7
  + Better career growth   → score 8
                               ———
  Positive Total: 24
```

### 📋 Step 2 — List the Negatives

On a **separate sheet**, write down all the negative points. Again, score each one **from 0 to 10**, but this time a **10 means it's a major drawback**.

```
  − Longer working hours   → score 6
  − Less vacation time     → score 4
  − Risky industry         → score 7
                               ———
  Negative Total: 17
```

### ⚖️ Step 3 — The 2:1 Verdict

Calculate the **ratio** of positives to negatives:

```
Ratio = Positive Total ÷ Negative Total
```

| Condition | Verdict | Meaning |
|---|---|---|
| **Ratio ≥ 2** | 🟢 **Do It!** | Positives outweigh negatives by at least 2‑to‑1. Go for it. |
| **1 ≤ Ratio < 2** | 🟡 **Think Twice** | Positives are ahead but haven't reached the 2:1 threshold. Proceed with caution. |
| **Ratio < 1** | 🔴 **Don't Do It** | Negatives dominate. This is clearly not the right move. |
| No factors entered | ⚪ **Pending** | Add factors to get your verdict. |

> _"If the positive score is at least double the negative score, you should do it — whatever 'it' is. But if the positives don't outweigh the negatives by that two‑to‑one ratio, don't do it, or at least think twice about it."_
>
> — Seymour Schulich

### 📊 Example

| Factor | Type | Score |
|---|---|---|
| 💰 Higher salary | Positive 👍 | 9 |
| 🚗 Shorter commute | Positive 👍 | 7 |
| 📈 Career growth | Positive 👍 | 8 |
| ⏰ Longer hours | Negative 👎 | 6 |
| 🏖️ Less vacation | Negative 👎 | 4 |
| ⚠️ Risky industry | Negative 👎 | 7 |

```
Positive Total = 9 + 7 + 8 = 24
Negative Total = 6 + 4 + 7 = 17
Ratio = 24 ÷ 17 ≈ 1.41

Verdict: 🟡 Think Twice (ratio is between 1 and 2)
```

---

## 🚀 Getting Started

The entire app is a **single HTML file** — no build tools, no dependencies (except Chart.js loaded via CDN).

### Option 1: Open directly

```bash
git clone https://github.com/GianfrancoPiazzolla/Decisions.git
cd Decisions
start index.html
```

### Option 2: Serve locally (recommended for full PWA support)

```bash
npx serve .
# or
python -m http.server 8080
```

Then open `http://localhost:8080` in your browser.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| **HTML5** | App structure |
| **CSS3** (custom properties, flexbox, grid) | Responsive UI with dark/light theme |
| **Vanilla JavaScript** (ES6+) | All app logic, no framework |
| **Chart.js 4** | Bar chart visualization |
| **Canvas 2D API** | Custom analog gauge rendering |
| **localStorage** | Persistent data storage |
| **Google Fonts** (Rajdhani, DM Sans, JetBrains Mono) | Typography |

---

## 🎨 Design Philosophy

The UI follows a **React Native‑inspired aesthetic** with:

- 🪟 **Glass‑morphism** (backdrop‑filter blur, semi‑transparent backgrounds)
- 🌈 **Gradient accents** (blue‑to‑cyan on headers, logo, buttons and FAB)
- 🔲 **Border‑radius throughout** (cards, buttons, inputs, modals)
- ✨ **Micro‑animations** (card entrances, ripple effects, toast notifications, bounce‑in FAB)
- 📐 **Rajdhani** for display/headings, **DM Sans** for body text, **JetBrains Mono** for numeric data
- 🌓 **Automatic dark/light mode** with smooth CSS transitions

---

## 🤝 Contributing

Contributions, issues and feature requests are welcome!  

1. 🍴 Fork the project
2. 🔀 Create your feature branch (`git checkout -b feature/amazing-feature`)
3. 💾 Commit your changes (`git commit -m 'Add amazing feature'`)
4. 📤 Push to the branch (`git push origin feature/amazing-feature`)
5. 📨 Open a Pull Request

---

## 📜 License

Distributed under the **MIT License**. Feel free to use, modify, and share.

---

> 🌱 *Made with ❤️ and 🧠. If you find this tool helpful, please leave a ⭐ on GitHub!*
