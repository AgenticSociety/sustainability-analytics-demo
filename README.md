# AI-Powered Sustainability Analytics — Interactive Demo

An interactive click-through demo showcasing **Conversational AI Analytics** with Microsoft Fabric Data Agents.

## What is this?

This demo simulates a live conversation with Claude AI, where two independent Fabric Data Agents (Revenue + Emissions) are combined through natural language to produce strategic sustainability insights — no dashboards, no ETL, just questions.

## Demo Beats

| Beat | Question | Insight |
|------|----------|---------|
| 1 | Show revenue by division | Portfolio overview from Revenue Agent |
| 2 | Biggest vs smallest emitter? | Emissions comparison from Emissions Agent |
| 3 | Revenue as a chart | AI generates the right visualization |
| 4 | Emissions intensity by revenue | **Derived metric** from both agents combined |
| 4b | Why is E-Mobility so high? | AI reasons about structural drivers |
| 5 | Priority quadrant | Strategic 2x2 matrix for capital allocation |
| 6 | Carbon price at €150/t | CFO-level margin impact simulation |
| 7 | Green revenue ratio | New ESG KPI born from the conversation |
| 8 | Cross-cutting use cases | 12 analytical use cases in 3 tiers |

## How to use

### Locally
```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/sustainability-analytics-demo.git
cd sustainability-analytics-demo

# Serve locally (any static server works)
python -m http.server 8000
# or
npx serve .
```

Open `http://localhost:8000` in your browser.

### GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to **main branch**, root `/`
4. Your demo will be live at `https://YOUR_USERNAME.github.io/sustainability-analytics-demo/`

## Navigation

- **Click** sidebar items to jump to any beat
- **→** or **Space** to advance
- **←** to go back
- **Esc** to reset to start

## Technology Stack

- **Data Layer**: Microsoft Fabric Lakehouse + Data Agents (MCP)
- **AI Layer**: Claude (Anthropic) with multi-agent orchestration
- **Visualization**: Chart.js, custom HTML/CSS
- **Hosting**: Static HTML — GitHub Pages compatible

## Architecture

```
User Question
     ↓
  Claude AI ←→ Fabric Revenue Agent (MCP)
     ↓      ←→ Fabric Emissions Agent (MCP)
  Derived Metrics + Reasoning
     ↓
  Interactive Visualization
```

The key insight: **the AI layer stays the same — it's the data that scales.** Every new dimension added to the Fabric Lakehouse unlocks exponentially more cross-cutting questions through the same conversational interface.

---

*Demo data for illustrative purposes. Built with Claude AI + Microsoft Fabric.*
