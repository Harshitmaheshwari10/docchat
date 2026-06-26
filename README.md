# DocChat — Smart Document Q&A

A free, browser-based document analysis app powered by Google Gemini.

## Features
- Upload multiple PDFs and TXT files
- Full PDF text extraction (via PDF.js, runs in-browser)
- Chat with your documents using AI
- Switch between documents or query all at once
- Quick actions: summarize, extract facts, find action items, compare docs
- Export chat as PDF or copy as text
- Works completely free — no server needed

## How to run

### Option 1 — Just open the file (easiest)
Double-click `docchat.html` — it opens directly in your browser. No install needed.

### Option 2 — Run with a local server (recommended for PDF support)
Some browsers block local file access. Use a simple server:

**With Python (built-in):**
```bash
python3 -m http.server 8080
```
Then open: http://localhost:8080/docchat.html

**With Node.js:**
```bash
npx serve .
```

## Setup
1. Get a free Gemini API key from https://aistudio.google.com/app/apikey
2. Paste it into the key field at the top of the app
3. Upload a PDF or TXT file and start chatting!

## Free tier limits
- 1,500 requests/day
- 1 million tokens/minute
- No credit card required

## Tech used
- Google Gemini 2.0 Flash (free API)
- PDF.js for in-browser PDF extraction
- Vanilla HTML/CSS/JS — zero dependencies to install
