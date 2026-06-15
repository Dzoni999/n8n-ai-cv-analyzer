# 📄 AI CV Analyzer

AI-powered CV Analyzer built with **n8n**, **LM Studio**, and **Qwen 3 4B**.

This workflow automatically extracts and analyzes information from PDF resumes, providing structured insights about a candidate's background, skills, experience level, strengths, and potential areas for improvement.

---

## ✨ Features

* 📄 Upload PDF resumes through a webhook
* 🤖 AI-powered CV analysis using a local LLM
* 🧠 Automatic candidate summary generation
* 🛠️ Skills extraction
* 📈 Experience level detection
* 💪 Strengths identification
* 🚀 Potential improvement area suggestions
* 🔗 Webhook-based API endpoint
* 💻 Runs locally with LM Studio

---

## 🏗️ Tech Stack

* n8n
* LM Studio
* Qwen 3 4B
* Webhooks
* PDF Text Extraction

---

## ⚙️ Workflow Overview

1. Receive a PDF resume via webhook.
2. Extract text from the PDF document.
3. Prepare and clean the CV content.
4. Analyze the resume using a local AI model.
5. Return a structured candidate analysis.

---

## 🔄 Workflow

```text
Webhook
↓
Extract From File
↓
Prepare CV
↓
Basic LLM Chain
↓
Respond To Webhook
```

---

## 📥 Example Response

```json
{
  "analysis": {
    "summary": "Junior Software Developer with experience in ASP.NET Core and databases.",
    "skills": [
      "C#",
      "ASP.NET Core",
      "SQL",
      "Git"
    ],
    "experience_level": "Junior",
    "strengths": [
      "Backend Development",
      "Problem Solving"
    ],
    "improvement_areas": [
      "Cloud Platforms",
      "Docker"
    ]
  }
}
```

---

## 🚀 Getting Started

### Prerequisites

* n8n installed locally
* LM Studio installed
* Qwen 3 4B model downloaded
* OpenAI-compatible API enabled in LM Studio

### Installation

1. Clone this repository.
2. Import `workflow.json` into n8n.
3. Configure the Chat Model node to use your LM Studio endpoint.
4. Load the Qwen model in LM Studio.
5. Activate the workflow.
6. Send a PDF resume to the webhook endpoint.

---

## 📸 Screenshot

<img src="workflow_ss.png" width="100%">

---

## 🎯 Purpose

This project was built to explore AI-powered workflow automation using n8n and local LLMs while solving a practical recruitment and resume analysis use case.

---

## 📄 License

MIT
