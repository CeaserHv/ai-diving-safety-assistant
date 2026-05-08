# AI-Powered Diving Safety Assistant

A constraint-grounded AI system for recreational diving safety analysis.

This project is an educational prototype that analyzes natural language dive plans, estimates risk levels, generates safety recommendations, and verifies outputs using rule-based and optional LLM-based reasoning.

---

## Project Overview

The system accepts a user query such as:

> I am a beginner and want to dive 32 meters for 40 minutes in 14°C water with strong current. What should I do?

It then performs:

1. Natural language parsing
2. Dive parameter extraction
3. Risk estimation
4. Recommendation generation
5. Constraint verification
6. Optional LLM reasoning
7. Final explanation generation
8. Web interface display (Gradio)

---

## Features

- Natural language dive plan input
- Regex-based parser (no API required)
- Optional LLM-based reasoning
- Risk scoring system
- Recommendation generation
- Safety verification layer
- Deterministic fallback
- Gradio web UI

---

# Quick Start (Run in Google Colab)

**This is the easiest way to run the project (no setup required)**

---

## Step 1: Open Google Colab

Go to:

https://colab.research.google.com/

---

## Step 2: Upload Notebook

Click:

File → Upload notebook

Then upload:

diving_safety_llm_colab_revised.ipynb

---

## Step 3: Install Dependencies

Run this cell:

```python
!pip -q install openai pandas matplotlib gradio
```

---

## Step 4: Run All Cells

Click:

Runtime → Run all

---

## Step 5: Launch the Web App

At the bottom of the notebook, you will see:

```python
demo.queue()
demo.launch(share=True)
```

After running, it will output:

Running on public URL: https://xxxx.gradio.live

Click the link

---

## Step 6: Use the App

Enter a dive plan like:

I am a beginner and want to dive 32 meters for 40 minutes in 14 C water with strong current. What should I do?

Click:

Analyze Dive Plan

---

## Step 7: View Results

The system will show:

🔴 Risk level
📌 Parsed Dive Plan
📊 Risk score
⚠️ Risk factors
🧭 Recommendations
✅ Verification results
🧠 Final explanation
⚠️ Disclaimer
