<div align="center">

# 🛡️ GEMINI SENTINEL

### AI-Agent Security Intelligence & Threat Detection

**Detect · Correlate · Reason · Respond**

A security monitoring and investigation platform for identifying suspicious
AI-agent behavior, correlating security findings, reconstructing attack
chains, and assisting incident analysis.

<br>

<a href="https://gemini-sentinel-6zhrw4jz66wpnnyxqz62ku.streamlit.app/">
  <img src="https://img.shields.io/badge/🚀_Live_Demo-Launch_Sentinel-FF4B4B?style=for-the-badge" alt="Live Demo">
</a>
<a href="https://github.com/mradulkrish911/Gemini-Sentinel">
  <img src="https://img.shields.io/badge/GitHub-Source_Code-181717?style=for-the-badge&logo=github" alt="GitHub Repository">
</a>

<br><br>

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit">
<img src="https://img.shields.io/badge/Google_Gemini-4285F4?style=flat-square&logo=googlegemini&logoColor=white" alt="Google Gemini">
<img src="https://img.shields.io/badge/AI-Agent_Security-7C3AED?style=flat-square" alt="AI Agent Security">

</div>

---

## 📌 Overview

**Gemini Sentinel** is an AI-agent security monitoring and investigation
platform designed to identify suspicious behavior, evaluate security
violations, reconstruct related attack activity, and support incident
investigation.

AI agents interact with tools, APIs, memory systems, and external content.
Individual actions may appear harmless in isolation, while a sequence of
related events can indicate a broader security incident.

Gemini Sentinel combines configurable rule-based detection, structured
incident analysis, attack-chain reconstruction, and AI-assisted explanations
to make suspicious agent activity easier to investigate.

The project uses synthetic security events to demonstrate its detection
and investigation workflow.

## ✨ Key Features

### 🔍 Rule-Based Threat Detection

- Evaluate security events against configurable rules.
- Identify tool-scope violations and missing approvals.
- Highlight suspicious high-risk agent actions.
- Organize detection results into security findings and incidents.

### 🧩 Incident Investigation

- Inspect incidents through an interactive dashboard.
- Review severity, risk scores, confidence scores, and finding counts.
- Examine security findings associated with individual incidents.
- Investigate suspicious agent activity through structured incident views.

### 🔗 Attack-Chain Reconstruction

- Organize related findings into reconstructed attack sequences.
- Investigate multi-stage suspicious activity.
- Examine relationships between security events.
- Understand how multiple security violations can form a broader attack scenario.

### 🤖 AI-Assisted Analysis

- Integrate Google Gemini for natural-language incident analysis.
- Help explain the significance of detected security activity.
- Supplement rule-based findings with AI-generated interpretations.
- Support fallback analysis when AI analysis is unavailable, where implemented.

### 🚨 Response Recommendations

- Present recommended security actions for suspicious incidents.
- Highlight response priorities.
- Provide incident-management controls for actions such as isolating an
  agent or resolving an incident.

> Response recommendations and dashboard controls should not be interpreted
> as proof of real-world containment unless the corresponding actions are
> connected to an operational enforcement system.

### 🧪 Synthetic Attack Simulation

- Generate synthetic security events for testing and demonstration.
- Explore scenarios involving suspicious external input, memory poisoning,
  unauthorized high-risk actions, and attempted evidence removal.
- Demonstrate investigation workflows without modifying real systems.

### 🎛️ Interactive Security Filters

- Filter displayed security information by agent and severity.
- Focus investigations on relevant events and findings.
- Navigate security information through the dashboard.

---

## 📸 Application Preview

To keep the README compact and avoid oversized screenshots, open each
image individually.

| Feature | Preview |
|---|---|
| Security Dashboard | [View Dashboard](assets/dashboard.png) |
| Incident Investigation | [View Incident Investigation](assets/incident-investigation.png) |
| Security Findings | [View Security Findings](assets/security-findings.png) |
| Attack-Chain Reconstruction | [View Attack Chain](assets/attack-chain.png) |
| Response Recommendations | [View Response Recommendations](assets/response-recommendations.png) |
| Security Filters | [View Security Filters](assets/security-filters.png) |

### 🛡️ Security Dashboard

Monitor event volume, detection findings, incident counts, severity metrics,
risk scores, and the incident investigation queue.

### 🔍 Incident Investigation

Inspect incident information and investigate suspicious agent activity.

### 🚨 Security Findings

Examine findings such as tool-scope violations and high-risk actions
performed without required human approval.

### 🔗 Attack-Chain Reconstruction

Investigate related security findings as a sequence to understand
potential multi-stage attack scenarios.

### ⚙️ Response Recommendations

Review recommended security actions, response priorities, and available
incident-management controls.

### 🎛️ Security Filters

Filter security information by agent and severity to focus on relevant
events and findings.

---

## 🏗️ Architecture

```text
                    GEMINI SENTINEL
                           |
                           v
                Synthetic Event Generator
                           |
                           v
                   JSONL Event Stream
                           |
                           v
                  Detection Pipeline <--- rules.yaml
                           |
                           v
                   Security Findings
                           |
                           v
                   Incident Analysis
                           |
                +----------+----------+
                |                     |
                v                     v
          Attack-Chain         Streamlit Dashboard
          Investigation               |
                                      v
                              Google Gemini API
                                      |
                                      v
                           AI-Assisted Explanation
                                      |
                                      v
                            Response Recommendations
```

### Workflow

1. **Generate:** Create synthetic security events for testing and demonstration.
2. **Ingest:** Process events from the JSONL event stream.
3. **Detect:** Evaluate events against configured security rules.
4. **Investigate:** Organize findings into incidents and reconstruct attack chains.
5. **Analyze:** Use Gemini to generate natural-language incident explanations
   when the AI integration is available.
6. **Respond:** Present recommended security actions and incident-management
   controls.

---

## 📊 Demonstration Metrics

The current demonstration dashboard displays:

| Metric | Displayed Value |
|---|---:|
| Events | 5,500 |
| Findings | 3,520 |
| Incidents | 172 |
| Critical / High | 170 / 0 |
| Average Risk | 98/100 |

These values represent the generated demonstration dataset and the
application's current output. They are not independently validated
production benchmarks or measurements of real-world detection accuracy.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core application and detection logic |
| Streamlit | Interactive security dashboard |
| Google Gemini API | AI-assisted incident analysis |
| YAML | Configurable detection rules |
| JSON / JSONL | Event and incident data |
| Git & GitHub | Version control and collaboration |
| Streamlit Community Cloud | Deployment |

---

## 📂 Project Structure

```text
Gemini-Sentinel/
├── assets/
│   ├── dashboard.png
│   ├── incident-investigation.png
│   ├── security-filters.png
│   ├── attack-chain.png
│   ├── security-findings.png
│   └── response-recommendations.png
├── app.py
├── detect.py
├── generate_events.py
├── generate_walkthrough_pdf.py
├── rules.yaml
├── requirements.txt
├── test_ai_integration.py
├── .env.example
├── .gitignore
└── README.md
```

---

## 🚀 Run Locally

### Prerequisites

- Python
- Git
- API credentials for AI-assisted analysis

### 1. Clone the repository

```bash
git clone https://github.com/mradulkrish911/Gemini-Sentinel.git
cd Gemini-Sentinel
```

### 2. Create a virtual environment

**Windows PowerShell**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API credentials

Use `.env.example` as a reference for configuring your local environment.

For Google Gemini, the expected environment variable may be:

```env
GEMINI_API_KEY=your_gemini_api_key
```

If your implementation also uses Grok, configure its API key using the
exact variable name expected by the code.

Never commit real API keys or `.env` files to GitHub.

For Streamlit Community Cloud, configure credentials through the
application's Secrets settings.

### 5. Launch the application

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal.

---

## 🔐 Security Considerations

Gemini Sentinel is a development and demonstration project for AI-agent
security monitoring.

- Synthetic attack scenarios are intended for testing and demonstration.
- Detection results depend on the supplied events and configured rules.
- AI-generated explanations may be incomplete or incorrect.
- API credentials must be stored securely.
- Response recommendations should be reviewed by a human.
- Actual agent isolation or containment requires integration with the
  relevant enforcement mechanisms.

The project is not a substitute for a production-grade security monitoring
or incident-response platform.

---

## 🗺️ Future Improvements

Potential areas for further development include:

- [ ] Expand detection coverage for additional AI-agent attack patterns.
- [ ] Improve correlation across multi-stage attack sequences.
- [ ] Add persistent incident history.
- [ ] Expand automated tests for detection rules and edge cases.
- [ ] Evaluate detection quality against labeled security-event datasets.
- [ ] Integrate with external logging and monitoring systems.
- [ ] Explore operational enforcement for supported response actions.

---

## 🌐 Live Demo

<div align="center">

### 🚀 [Launch Gemini Sentinel](https://gemini-sentinel-6zhrw4jz66wpnnyxqz62ku.streamlit.app/)

Explore the dashboard, inspect security findings, investigate reconstructed
attack chains, and review recommended responses.

</div>

AI-assisted analysis requires correctly configured API credentials and
availability of the external AI service.

---

<div align="center">

### 🛡️ GEMINI SENTINEL

**From Security Events to Actionable Intelligence**

Detect · Correlate · Reason · Respond

</div>
