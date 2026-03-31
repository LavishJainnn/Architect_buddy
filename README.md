# 🏡 AI Home Renovation Multi-Agent System

A powerful multi-agent AI system built with **Google ADK** that analyzes your room photos, creates personalized renovation plans, and generates **photorealistic renderings** using **Gemini 3 Flash** and **Gemini 3 Pro** multimodal capabilities.

---

## 🚀 Overview

This project demonstrates a **production-style multi-agent architecture** where specialized AI agents collaborate to:

* Analyze your space
* Understand your design preferences
* Plan renovations within your budget
* Generate realistic visual previews

It uses a **Coordinator/Dispatcher + Sequential Pipeline pattern** to efficiently orchestrate tasks.

---

## ✨ Features

* 🔍 **Smart Image Analysis**
  Upload room photos and inspiration images — the system automatically detects and analyzes them

* 🎨 **Photorealistic Rendering**
  Generate high-quality images of your renovated space using Gemini 3 Pro

* 💰 **Budget-Aware Planning**
  Tailored recommendations based on your budget constraints

* 📊 **Complete Renovation Roadmap**
  Includes timeline, cost breakdown, contractor suggestions, and action checklist

* 🤖 **Multi-Agent Orchestration**
  Demonstrates real-world agent patterns (Coordinator + Pipeline)

* ✏️ **Iterative Refinement**
  Modify renderings through natural language feedback

---

## 🧠 How It Works

The system uses three specialized agents coordinated by a central dispatcher:

### 📸 Visual Assessor

* Analyzes uploaded room images (layout, condition, dimensions)
* Extracts style from inspiration images
* Identifies improvement opportunities and estimates costs

---

### 🎨 Design Planner

* Creates budget-conscious design plans
* Specifies materials, colors, fixtures
* Prioritizes high-impact upgrades

---

### 🏗️ Project Coordinator

* Generates full renovation roadmap
* Produces photorealistic renderings
* Provides timeline, cost breakdown, and actionable steps

---

## ⚙️ Multi-Agent Architecture

```
Coordinator (Root Agent)
    ├── Info Agent (quick Q&A)
    └── Planning Pipeline (Sequential)
          ├── Visual Assessor (image analysis)
          ├── Design Planner (specifications)
          └── Project Coordinator (rendering + roadmap)
```

### Why this pattern?

* ⚡ Efficient → Runs only necessary workflows
* 🧩 Modular → Each agent has a clear responsibility
* 📈 Scalable → Easy to extend with new features
* 🏭 Production-ready → Mirrors real-world AI systems

---

## 🛠️ Installation

### 1. Clone or Download the Repository

* Clone via Git
* OR download as ZIP and extract

---

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Setup API Key

You need a **Google Gemini API key**.

### On macOS/Linux:

```bash
export GOOGLE_API_KEY="your_gemini_api_key"
```

### OR create a `.env` file:

```
GOOGLE_API_KEY=your_gemini_api_key
```

---

## ▶️ Running the Project

```bash
cd multi_agent_apps
adk web
```

---

## 🌐 Access the Application

1. Open your browser
2. Select: **ai_home_renovation_agent**
3. Start interacting with your AI renovation assistant 🎉

---

## 💡 Usage Examples

### 🏠 Scenario 1: Room + Budget

Upload your room image and ask:

```
"What can I improve here with a $5k budget?"
```

→ Get budget-friendly suggestions + rendering

---

### 🎯 Scenario 2: Room + Inspiration

Upload:

* Your room
* Inspiration image (Pinterest, etc.)

```
"Transform my kitchen to look like this. What's the cost?"
```

→ Style transfer + cost estimation + rendering

---

### 📝 Scenario 3: Text-Based Input

```
"Renovate my 10x12 kitchen with oak cabinets and laminate counters. 
Modern farmhouse style. Budget: $30k"
```

→ Full plan + generated visualization

---

### 🔄 Scenario 4: Iterative Refinement

After rendering:

```
"Make the cabinets cream instead of white"
"Add pendant lights"
"Change flooring to lighter oak"
```

→ Updated renderings based on feedback

---

## 🧪 Sample Prompts

* "Renovate my 8x12 kitchen with modern farmhouse style. Budget: $25k"
* "Turn my 5x8 bathroom into a spa-like retreat. Budget: $15k"
* "Make my bedroom cozy with accent wall and new flooring. Budget: $12k"

---

## 🧰 Tools & Capabilities

* 🔎 `google_search` → Finds trends, materials, pricing
* 💰 `estimate_renovation_cost` → Cost estimation by scope
* ⏱️ `calculate_timeline` → Project duration estimation
* 🖼️ `generate_renovation_rendering` → Image generation
* ✏️ `edit_renovation_rendering` → Iterative updates
* 🧾 Versioned artifacts → Tracks all generated outputs

---

## 📦 Tech Stack

* Python 🐍
* Google ADK
* Gemini 3 Flash & Gemini 3 Pro
* Multimodal AI (vision + text)

---

## ⚠️ Disclaimer

This project is for **educational and demonstration purposes only**.
Renovation costs and recommendations may vary in real-world scenarios.

---

## 🚀 Future Improvements

* Add React-based frontend dashboard
* Integrate real contractor APIs
* Add AR/VR visualization support
* Deploy as SaaS product

---

## ⭐ Support

If you found this project useful, give it a ⭐ and share it!

---
