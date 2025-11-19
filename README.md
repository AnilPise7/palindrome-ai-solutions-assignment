# AI Solutions Engineer Interview Assignment – Palindrome Data

This repository contains my submission for the **AI Solutions Engineer Assessment** from **Palindrome Data**.  
The objective is to analyse synthetic WhatsApp-style health conversations using Python and generate:

1. **Risk scores** for:
   - HIV acquisition  
   - Mental-health disorder indicators  
2. **A structured recommendation & care plan** aligned with high-level South African NDOH-style guidance  
3. **A reproducible, single-file Jupyter Notebook** demonstrating data processing, analysis, and reasoning 

---

## 📁 Repository Structure

```text
├── pal_ai_solutions_assignment.ipynb      # Main notebook (required submission)
├── health_ai_whatsapp_100_conversations_long.txt
├── conversation_risk_scores_and_plans.csv
└── README.md
```

---

## 🚀 Features of the Notebook

### ✅ 1. Data Ingestion & Parsing
- Reads WhatsApp-style synthetic conversations  
- Parses timestamp, speaker, and utterance  
- Structures messages into a DataFrame  
- Aggregates user text per conversation for risk analysis  

### ✅ 2. Explainable Rule-Based Risk Model
- HIV risk scored using weighted keyword signals  
- Mental-health risk scored using crisis and moderate indicators  
- Normalised scores mapped into **low / moderate / high** categories  
- Fully transparent, interpretable heuristics suitable for interview evaluation  

### ✅ 3. Recommendation & Care Plan Generator
For each conversation:
- Summarises detected behavioural & emotional indicators  
- Generates a structured, non-prescriptive plan that includes:  
  - HIV testing / prevention guidance  
  - Stress / mood support steps  
  - Emergency escalation pathways when crisis language appears  

### ✅ 4. Visualisation & Case Inspection Tools
- Function `show_conversation()` allows interactive review of:  
  - Message history  
  - Computed risk scores  
  - Generated plan  

### ✅ 5. Exported Output
- `conversation_risk_scores_and_plans.csv` – contains risk scores + recommendations for all conversations  

---

## 🧠 Design Choices

- **Rule-based modelling** for complete transparency in a healthcare-related context  
- **Keyword lexicons** to approximate intent detection without labelled training data  
- Notebook structured to emphasise:  
  - Logic clarity  
  - Reproducibility  
  - Readable, modular code  
  - Interview-friendly reasoning  

---

## 📌 Limitations (Acknowledged in Notebook)
- Not clinically validated  
- Designed only as a prototype for the assessment  
- Any real deployment would require:  
  - Medical expert review  
  - Model calibration  
  - Safety guardrails  
  - Escalation logic  

---

## 🕒 Time Spent
Documented inside the notebook, as requested.

---

## 👤 Author
**Anil Pise**  
Senior Data Scientist  
Email: `anilapise7@gmail.com`
