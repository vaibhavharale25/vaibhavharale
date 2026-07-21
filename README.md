# 🩺 AuraHealth AI - Generative AI Health Assistant

> **A dynamic, Generative AI (GenAI)-powered web application providing reliable health awareness, symptom explanations, preventive wellness planning, and medical term simplification with responsible AI safety guardrails.**

---

## ⚠️ Important Medical Disclaimer

**AuraHealth AI is built strictly for educational health awareness and informational purposes.** 
- It is **not** a substitute for professional medical advice, diagnosis, or treatment.
- Always consult a qualified physician or healthcare provider for personal health decisions.
- **In an emergency**, call your regional emergency service (e.g., 911, 999, 112, 108) immediately.

---

## ✨ Core Features & Functionality

### 🤖 1. Interactive Symptom AI Chatbot
- **Real-Time Streaming Responses**: Real-time token streaming for a dynamic AI interaction experience.
- **Audio Text-to-Speech (TTS)**: Listen to generated health guidance directly in the browser.
- **Quick Prompt Pills**: Instant starter queries for common health concerns.
- **One-Click Copy & Clipboard**: Easily copy response summaries for personal logs.

### 🫀 2. Interactive Visual Body Symptom Selector
- **Anatomical Mapping**: Clickable body regions (**Head & Cranial**, **Throat & Neck**, **Chest & Respiratory**, **Abdomen & Digestive**, **Back & Spine**, **Joints & Limbs**).
- **Targeted Symptom Analysis**: Select specific symptoms (e.g. *Shortness of breath*, *Acid reflux*) to auto-populate context for GenAI analysis.

### 🛡️ 3. GenAI Emergency Red-Flag Triage
- **Automated Keyword Scanner**: Scans user queries in real-time for acute symptoms indicating cardiac, respiratory, or neurological crises.
- **Urgent Safety Modal**: Automatically opens a high-priority Red-Flag Alert Modal with emergency advice and direct regional hotline numbers (911, 999, 112, 108).

### 📋 4. Preventive Wellness & Screening Planner
- **Age-Tailored Checklists**: Generates routine medical screening recommendations for **18-29**, **30-44**, **45-64**, and **65+** age brackets.
- **Lifestyle & Disease Prevention**: Customized daily habits for heart health, sleep hygiene, joint mobility, and stress management.

### 📖 5. Medical Term & Lab Result Simplifier
- **Jargon Translation**: Translates complex clinical terms (*Hyperlipidemia*, *TSH*, *Leukocytosis*, *HbA1c*, *Idiopathic*) into plain, easy-to-understand language.

### 📄 6. Printable Health Summary Exporter
- **Doctor Appointment Report**: Formatted printable/downloadable PDF report capturing patient queries and AI summaries to facilitate clinical intake discussions.

---

## ⚡ Dual AI Engine Architecture

AuraHealth AI features a flexible dual-engine strategy:

1. **Built-in Intelligent GenAI Engine** *(Default)*:
   - Works 100% out of the box with zero external API key dependencies or setup.
   - Provides multi-perspective health answers, differential cause lists, preventive tips, and follow-up prompts.
2. **Google Gemini Live API Integration**:
   - Supports custom Google Gemini API keys (`gemini-1.5-flash` / `gemini-1.5-pro`) directly via the in-app **Settings Modal** (`⚙️`).
   - Client-side key storage in `localStorage` — keys are never sent to external third-party servers.

---

## 🛠️ Technology Stack

- **Frontend Framework**: [React 18](https://react.dev/) + [Vite](https://vitejs.dev/)
- **UI Design System**: Vanilla CSS with modern Glassmorphism, CSS Variables, dark/light theme tokens, and micro-animations
- **Iconography**: [Lucide React](https://lucide.dev/)
- **Generative AI Core**: Custom JS AI synthesis controller & Google Gemini REST API streaming

---

## 🚀 Quick Start Guide

### Prerequisites
- Node.js (v18.0.0 or higher)
- npm (v9.0.0 or higher)

### Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/vaibhavharale25/harale.git
   cd harale
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the local development server**:
   ```bash
   npm run dev
   ```
   Open your browser and navigate to `http://localhost:3000`.

4. **Build for production**:
   ```bash
   npm run build
   ```

---

## 📂 Project Structure

```text
├── index.html                    # HTML entry point with fonts & SEO meta tags
├── package.json                  # Dependencies & scripts
├── vite.config.js                # Vite configuration
└── src/
    ├── main.jsx                  # React DOM root entry
    ├── App.jsx                   # Main state manager & modal container
    ├── index.css                 # Glassmorphism design tokens & styles
    ├── services/
    │   └── aiEngine.js           # Core GenAI controller & emergency triage
    ├── data/
    │   └── medicalKnowledge.js   # Clinical knowledge base & red-flag rules
    └── components/
        ├── Navbar.jsx            # Main navigation & header
        ├── DisclaimerBanner.jsx  # Top sticky medical disclaimer strip
        ├── SymptomChat.jsx       # Interactive AI chatbot component
        ├── BodyMap.jsx           # Visual anatomical symptom selector
        ├── PreventiveCarePlanner.jsx # Age-tailored wellness planner
        ├── TermSimplifier.jsx    # Medical jargon simplifier
        ├── EmergencyAlertModal.jsx # Red-flag emergency alert modal
        ├── ApiSettingsModal.jsx  # Gemini API key configuration modal
        └── ExportSummaryModal.jsx # Printable doctor consultation summary
```

---

## 📜 Responsible AI & Safety Standards

- **Transparency**: Clear disclosures on AI limitations across all views.
- **Privacy First**: No patient identifiers or health logs are transmitted or stored on external backend servers.
- **Safety First**: Non-diagnostic language enforced on all synthesized outputs.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
