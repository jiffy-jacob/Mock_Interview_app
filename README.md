# 🎤 AI Interview Coach

A resume-based mock interview app. Upload your resume, choose a role and round (Technical or HR), and answer by voice. Get feedback and an improved answer after each question, plus an overall score out of 5.

**Live app:** *https://mockinterviewapp-zxfauwpcjqcxerydbrfvbx.streamlit.app/*

## Features

- Questions based on your resume and chosen role, different every run
- Technical and HR rounds, unlimited questions until you press **Exit**
- Voice answers with editable text
- Feedback and improved answer after each question
- Overall score out of 5

## Tech Stack

Streamlit · Groq API (LLM + Whisper speech-to-text) · TF-IDF retrieval (scikit-learn) · pypdf

## Setup

Requires Python 3.10+ and a free [Groq API key](https://console.groq.com/keys).

```bash
git clone <your-repo-url>
cd <your-repo-folder>
pip install -r requirements.txt
```

Create `.streamlit/secrets.toml`:

```toml
GROQ_API_KEY = "your_key_here"
```

Run:

```bash
streamlit run app.py
```

Optional: add interview-prep PDFs to a `knowledge_base/` folder next to `app.py`.

## Deploy

Push the repo to GitHub, create an app on [Streamlit Community Cloud](https://share.streamlit.io) with `app.py` as the main file, and add `GROQ_API_KEY` under **Settings → Secrets**.

## Author

**Jiffy Jacob**

