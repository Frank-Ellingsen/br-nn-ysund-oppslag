# Brønnøysund AI Financial Intelligence & S-Curve Prognosis

An AI-powered web application for real-time Norwegian company lookup via the official **Brønnøysundregisteret API (Enhetsregisteret)**, integrated with **Google Gemini AI** for strategic financial diagnosis, action recommendations, and predictive **S-Curve financial prognosis modeling**.

![Brønnøysund AI Application Screenshot](https://raw.githubusercontent.com/frank-ellingsen/Look_Up_Bronnoysund/main/docs/app_preview.png)

---

## 🌟 Key Features

1. **Live Norwegian Entity Lookup (Brønnøysund Enhetsregisteret API)**
   - Search any Norwegian entity by company name or 9-digit organization number (`orgnr`).
   - Fetches live official registration details: Name, Org Form, Industry Næringskode, Number of Employees, Registration Date, Registered Municipality, MVA status, and Liquidation/Bankruptcy status.
   - Quick preset lookup buttons for sample Norwegian enterprises (e.g. *AMOK EQUIPMENT AS*, *UMOE MANDAL AS*, *EQUINOR ASA*, *KONGSBERG GRUPPEN ASA*).

2. **AI Engine & API Key Integration**
   - Configurable AI Provider selection (Default: **Google Gemini AI 2.5 Flash**).
   - Direct client-side API integration using your own Gemini API Key (saved securely in browser `localStorage`).
   - Built-in fallback financial controller logic if no API key is provided, ensuring uninterrupted functionality.

3. **Strategic AI Action Recommendations**
   - Generates categorized strategic recommendations based on company size, industry, and baseline financial performance:
     - **Cost Optimization & EAC Risk Mitigation**: Project Estimate-at-Completion gate checks.
     - **Working Capital Optimization**: DSO reduction and milestone billing acceleration.
     - **Revenue Expansion**: High-margin recurring service attachments.
     - **Risk Mitigation**: FX and material price hedging.

4. **Predictive S-Curve Prognosis Modeling**
   - Compares **Current Baseline Trajectory** vs. **AI-Recommended Action Prognosis**.
   - Interactive Chart.js S-Curve visualizing 12-month cumulative free cash flow realization.
   - KPI comparison metrics: Revenue impact %, EBITDA margin expansion (bps), Net Cash Flow delta, and Mitigated Project EAC cost overruns.
   - **Tufte-Style 3-Statement Financial Table**: Clean left-aligned text, right-aligned monospaced figures, no vertical gridlines, and clear variance highlighting.

---

## 🚀 How to Run Locally

Because this application is built with modern HTML5, CSS3, and vanilla JavaScript using public CORS-enabled APIs, no build tools or servers are required!

1. Clone or download this repository:
   ```bash
   git clone https://github.com/frank-ellingsen/Look_Up_Bronnoysund.git
   cd Look_Up_Bronnoysund
   ```
2. Open `index.html` in any web browser (Chrome, Edge, Firefox, Safari).

---

## 🔑 Setting Up Gemini AI Key

1. Get a free API key from [Google AI Studio](https://aistudio.google.com/).
2. Open the application, enter your key in the **Gemini API Key** field, and click **Run Strategic AI Diagnosis & S-Curve Prognosis**.
3. Your key is stored locally in your browser's `localStorage` and never sent to any third-party server.

---

## 🌐 Publishing to GitHub Pages

This repository includes a automated GitHub Actions workflow (`.github/workflows/deploy-pages.yml`).

### Automatic Deployment:
1. Create a new repository on GitHub named `Look_Up_Bronnoysund`.
2. Link your local repo and push to the `main` branch:
   ```bash
   git remote add origin https://github.com/YOUR_GITHUB_USERNAME/Look_Up_Bronnoysund.git
   git branch -M main
   git push -u origin main
   ```
3. In your GitHub repository settings:
   - Go to **Settings** -> **Pages**.
   - Under **Source**, select **GitHub Actions**.
4. The workflow will automatically publish your site to `https://YOUR_GITHUB_USERNAME.github.io/Look_Up_Bronnoysund/`.

---

## 🛠️ Technology Stack

- **Frontend**: HTML5, Vanilla CSS3 (Custom Design System with Slate/Zinc palette), Modern JavaScript (ES6+).
- **APIs**: Brønnøysundregisteret Open REST API (`data.brreg.no`), Google Gemini REST API (`generativelanguage.googleapis.com`).
- **Visualization**: Chart.js 4.4 for S-Curve rendering.
- **Design Principles**: Edward Tufte Data-Ink Ratio compliance.

---

## 📄 License

MIT License. Developed for financial controllers, project controllers, and business intelligence specialists.
