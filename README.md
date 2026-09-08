# ⚡ Inuka Fellowship Hackathon — Judge Evaluation Portal

> **Power Learn Project** · Hackathon Evaluation System  
> *Powering communities through technology, learning, and innovation.*

---

## 📖 Overview

A sleek, responsive web application designed to help judges evaluate hackathon projects during **Stage 2** of the Inuka Fellowship Hackathon. The portal provides a streamlined interface for scoring teams across five weighted criteria, aggregating results, and generating ranked leaderboards — all branded with the vibrant **Power Learn Project** identity.

---

## ✨ Features

### 🎯 Judge Scoring
- **8 participating teams** with unique icons and color coding
- **5 weighted criteria** with interactive sliders (0–100)
- **Real-time score calculation** with weighted totals
- **Persistent notes** per team for qualitative feedback
- **Auto-save** to browser localStorage

### 🏆 Leaderboard
- **Animated podium** for top 3 teams
- **Full ranking table** with per-criterion breakdown
- **Color-coded scores** matching each criterion
- **One-click refresh** to update rankings

### 📋 Rubric Guide
- Detailed descriptions for each criterion
- Weight percentages clearly displayed
- Reference for judges during evaluation

###  Data Management
- **CSV Export** of all scores and notes
- **Reset functionality** with confirmation
- **LocalStorage persistence** across sessions

---

## 🎨 Design & Branding

The portal is themed around the **Power Learn Project** visual identity:

| Color | Hex | Usage |
|-------|-----|-------|
| ⚡ Cyan | `#00d4ff` | Primary accents, Relevance criterion |
| 🟣 Purple | `#7c4dff` | Secondary accents, Technical criterion |
| 🔴 Magenta | `#e91e63` | Highlights, Insight criterion |
| 🟠 Orange | `#ff9800` | Warm accents, Usability criterion |
| 🟢 Teal | `#00e5c8` | Success states, Presentation criterion |
| 🌑 Navy | `#0d1b3e` | Background base |

**Design elements inspired by PLP logos:**
- African-inspired animated gradient borders
- Network-dot background pattern (representing connectivity across Africa)
- Glowing slider thumbs with gradient fills
- Glassmorphism cards with subtle backdrop blur

---

## 🛠️ Tech Stack

- **HTML5** — Semantic structure
- **Tailwind CSS** (via CDN) — Utility-first styling
- **Custom CSS** — Animations, gradients, glassmorphism
- **Vanilla JavaScript** — All interactivity (no frameworks)
- **LocalStorage API** — Client-side data persistence

**Zero build step required** — runs directly in any modern browser.

---

##  Getting Started

### Option 1: Direct Open
Simply open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge).

### Option 2: Local Server
```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```
Then navigate to `http://localhost:8000`

### Option 3: Deploy
Deploy to any static hosting service:
- **GitHub Pages** — Push to a repo, enable Pages
- **Netlify** — Drag & drop the folder
- **Vercel** — Import the repository
- **Cloudflare Pages** — Connect your repo

---

## 📋 Grading Rubric

Stage 2 accounts for **35% of the total score**. Focus areas: *Analytics, Automation, AI, and User Experience*.

| Criterion | Weight | What Judges Look For |
|-----------|--------|----------------------|
| 🎯 **Relevance to Inuka Impact & Efficiency** | 25% | Addresses problem statements, improves beneficiary experience, focused scope |
| ⚙️ **Technical Quality & Integration** | 25% | Builds on Stage 1 data, offline-sync, defensible AI, reliable APIs, QA/UAT |
| 📊 **Insight, M&E Value & Quantified ROI** | 20% | Quantified benefits, honest assumptions, clear cost-benefit narrative |
| 📱 **Usability, Accessibility & Deployability** | 15% | Mobile-first, offline-capable, multilingual, pilot-ready |
| 🎤 **Presentation & Storytelling** | 15% | Clear communication, connects tech to human impact |

---

## 👥 Participating Teams

| # | Team | Icon |
|---|------|------|
| 1 | Apex Innovators | 🚀 |
| 2 | Avengers |  |
| 3 | FTG |  |
| 4 | Gen-Tech |  |
| 5 | Null Terminators | 🔴 |
| 6 | Scaffold | ️ |
| 7 | Synergy |  |
| 8 | Vertex G | 💎 |

---

## 📁 File Structure

```
inuka-judge-portal/
├── index.html          # Single-file application (HTML + CSS + JS)
└── README.md           # This file
```

> The entire application is contained in a single `index.html` file for easy deployment and sharing.

---

## 🧪 Usage Guide for Judges

1. **Select a team** from the grid at the top
2. **Adjust sliders** for each of the 5 criteria (0–100)
3. **Add notes** in the text area (optional)
4. **Click "Save Scores"** to persist to localStorage
5. **Repeat** for all 8 teams
6. **Switch to Leaderboard tab** to view rankings
7. **Export CSV** when judging is complete

### Scoring Tips
- Use the full 0–100 range for differentiation
- Consider the weight of each criterion when scoring
- Notes are included in the CSV export for reference

---

## 🔧 Customization

### Adding a New Team
Edit the `TEAMS` array in the `<script>` section:
```javascript
{ id: 'newteam', name: 'New Team Name', icon: '🌟', color: '#hexcolor' }
```

### Modifying Criteria Weights
Edit the `CRITERIA` array. Ensure weights sum to **100**:
```javascript
{ id: 'criterion', name: 'Name', weight: 25, icon: '🎯', color: '#hex', description: '...' }
```

### Changing Theme Colors
Update the CSS custom properties in `:root`:
```css
:root {
  --plp-cyan: #00d4ff;
  --plp-purple: #7c4dff;
  /* ... */
}
```

---

## 📊 Data Storage

- All scores are stored in **browser localStorage** under the key `inuka_plp_scores`
- Data persists across page refreshes and browser sessions
- Clearing browser data will reset scores
- Use **Export CSV** to back up scores externally

---

## 🌐 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 80+ | ✅ Full support |
| Firefox | 78+ | ✅ Full support |
| Safari | 14+ | ✅ Full support |
| Edge | 80+ | ✅ Full support |
| Mobile browsers | Modern | ✅ Responsive |

---

## 📝 License

This project is created for the **Inuka Fellowship Hackathon** under the **Power Learn Project** initiative.

---

## 🤝 Credits

- **Design inspiration**: Power Learn Project brand identity
- **Hashtag**: `#PowerCommunity`
- **Event**: Inuka Fellowship Hackathon

---

> ⚡ *Empowering African innovators to build solutions that matter.*
