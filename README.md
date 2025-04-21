# 🌱 FocusFlow – Grow Your Time. Grow Yourself.

> **A mindful, AI-assisted calendar app to track, plan, and visualize your effort.**  
> One hour a day, one branch at a time.

## ✨ Project Overview

**FocusFlow** helps you visualize how your time becomes progress.  
Instead of a rigid to-do list, you:
- Reflect on your **interests and goals each month**
- Let AI help you **plan what to do daily**
- Track your hours as **"energy invested"**
- Watch your efforts grow into a **tree-like visual timeline**

It's a calendar.  
It's a habit tracker.  
It's a personal growth journal — powered by time.

## 🌳 Metaphor: The Tree of Focus

- Each **hour** of effort is a **leaf** or **branch** grown.
- Every **interest** (e.g., English, Drawing, Fitness) is a **growth ring**.
- Daily effort is visualized as **circles of light**, **heat maps**, or a **blooming animation**.
- Focus is not about perfection — it's about showing up. Even 1 hour matters.

## 🧠 Core Features

### 1. 📆 Calendar View (Monthly Focus Dashboard)
- Users start from a familiar **monthly calendar**
- Each date shows:
  - Color-coded circles representing **hours spent**
  - A badge or tag for **primary interest of the day**
- **Clicking a day** expands:
  - AI-generated schedule
  - Notes & time logs

### 2. ✏️ Monthly Focus & Goal Setting
- Each month begins with:
  - "What do you want to focus on this month?"
  - Select or write down your interests (e.g. Language, Art, Study)
- You can track growth per interest

### 3. 🔮 AI-Powered Daily Plan Generator
- Each morning (or on demand), AI suggests:
  - A time-blocked schedule based on:
    - Your available time
    - Your monthly focus
    - Your energy preference (deep work / light work)
- Users can edit or follow as is

### 4. ⏳ Time Logging by Hour
- Each hour you invest = a visual increment
- You can:
  - Mark completed blocks
  - Add custom notes
  - Use a Pomodoro mode for built-in timer

### 5. 🌿 Effort Visualization Tree (Gamified Tracker)
- Cumulative effort appears as:
  - A **growing tree diagram**
  - A **radial sunburst or leaf map**
  - A **heatmap calendar (GitHub style)**
- Each interest has its own branch
- Hovering over segments shows detailed hour totals

### 6. 📤 Export & Sync
- Download `.ics` calendar
- Export weekly focus report
- Optional Google Calendar sync

## 🧩 Component Architecture

```bash
src/
├── components/
│   ├── CalendarView.jsx           # Monthly view with per-day effort dots
│   ├── DayDetailModal.jsx         # AI schedule + logs per day
│   ├── MonthlyFocusInput.jsx      # Set interests for the month
│   ├── PlanGenerator.jsx          # AI-generated schedule
│   ├── TimeLogger.jsx             # Log completed hours
│   └── GrowthVisualizer.jsx       # Tree or graph visualization of effort
├── utils/
│   ├── scheduler.js               # Time allocation based on availability & interest
│   └── treeBuilder.js             # Convert logs into visual growth
├── hooks/
│   ├── useCalendar.js             # Tracks active month/day
│   ├── useTimeBlocks.js           # For selecting & logging time
│   └── useAIPlanner.js            # Fetches AI suggestions
├── assets/
│   └── tree.svg / icons           # Visual elements
├── App.jsx
└── index.css
```

## 📦 Technical Stack

| Category      | Tech                            |
|---------------|---------------------------------|
| Framework     | React + Vite                    |
| Styling       | Tailwind CSS                    |
| State Mgmt    | `useState`, possibly `zustand`  |
| Visuals       | SVG + Canvas + D3 / Chart.js    |
| AI Integration| ChatGPT / Cursor-internal tools |
| Export        | `.ics` file format              |

## 🛠 Roadmap

| Phase | Features |
|-------|----------|
| MVP   | Calendar view + time logger + AI planner |
| v1.1  | Monthly focus + growth tree              |
| v1.2  | Heatmap visualization + weekly reports   |
| v2.0  | User login, sync, cross-device tracking  |

## 🙌 Author

**Tianru (Tiro) Peng**  
- CSCI 6809 – Assignment 2  
- Built with Cursor + GPT support  
- Vancouver, BC – 2025

## 💬 Philosophy

> "You don't need 10 hours. You need 1 hour of true focus. Then another."  
> Time itself is growth. This app makes your effort visible.
