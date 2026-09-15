# 🚀 [GridGuard — Power Outage Prediction & Grid Equipment Failure Advisor

IBM BoB AI Innovation Hackathon 2026 · Problem Statement **U1** (Utilities — Power, Energy, Transmission & Distribution)
]

> ⚠️ **Replace everything in `[ ]` brackets with your actual content before submission.**

---

## 👥 Team

| Field | Value |
|---|---|
| **Team Name** | [codex] |
| **Track** | [AI] |
| **Team Lead** | [Rutvi Ranparia] — [25ce100@charusat.edu.in] |
| **Members** | [Yati Soliya], [Rashi Domadiya], [Shivangi Tank] |

---

## 🎯 Problem Statement

> In 2–3 sentences: What problem does your project solve? Who experiences this problem?

[Describe the real-world problem your project addresses. Be specific about who the user is and what pain point they face.]

---

## 💡 Solution

> In 2–3 sentences: What did you build? How does it solve the problem above?

[Describe your solution clearly. Explain the core mechanism — what makes it work.]

---

## ✨ Key Features

- **Feature 1:** [Brief description — e.g., "Real-time anomaly detection using watsonx.ai"]
- **Feature 2:** [Brief description]
- **Feature 3:** [Brief description]
- **Feature 4:** [Optional]
- **Feature 5:** [Optional]

---

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| **Languages** | [Python 3.11, pandas, scikit-learn (Isolation Forest for anomaly detection)] |
| **Frameworks** | [IBM Bob (architecture planning, code review, natural-language summary generation)] |
| **IBM Technologies** | [watsonx.ai Granite (explanation/report generation layer)] |
| **Databases** | [Sample data in CSV to keep the demo runnable with no external accounts] |

## 📁 Repository Structure

```
├── src/                  # All source code
├── docs/                 # Written documentation
│   ├── problem-statement.md
│   ├── solution-overview.md
│   ├── architecture.md
│   └── setup-guide.md
├── demo/                 # Demo artifacts
│   ├── screenshots/      # App screenshots
│   └── demo-video-link.txt  # Link to demo video
├── presentation/         # Slide deck
└── submission.yaml       # Structured submission metadata
```

---

## ⚡ How to Run

> **Copy these exact steps from your [`docs/setup-guide.md`](docs/setup-guide.md)**

```bash
```bash
cd src
pip install -r requirements.txt
python main.py
```

This reads the sample data in `src/sample_data/`, prints a ranked risk table,
and writes `outage_risk_report.md` — the same report a grid ops supervisor
would receive.

---

## 🖥️ Demo

| Artifact | Link |
|---|---|
| 📹 Demo Video | [See demo/demo-video-link.txt](demo/demo-video-link.txt) |
| 🌐 Live Demo | [See demo/live-demo-url.txt](demo/live-demo-url.txt) |
| 🖼️ Screenshots | [See demo/screenshots/](demo/screenshots/) |
| 📊 Presentation | [See presentation/slides.pdf](presentation/) |

---

## ⚠️ Known Limitations

> Be honest — judges appreciate transparency over overclaiming.

- [Limitation 1: Sample data is synthetic (shaped like real SCADA/HUMS-style feeds) — it is
  not connected to a live utility's sensor network for this hackathon build."]
- [Limitation 2: The watsonx.ai explanation step currently runs against a mocked response in
  the demo build so it works without live credentials; the integration point
  is isolated in `src/main.py` (`generate_explanation()`), ready to swap in a
  real API key."]
- [Limitation 3: Crew pre-positioning currently assumes a single depot per region; multi-depot
  routing is on our roadmap, not in this build."]

---

## 🏅 What We're Most Proud Of

[The risk score isn't a single black-box number — every flagged asset gets a
plain-English "why" so a supervisor doesn't have to trust a number blindly.
That explainability layer is what actually makes this usable during a live
storm response, not just in a demo.]

---
