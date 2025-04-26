## 🚀Consulting Proposal Quality Checker
A modular, AI-powered application to analyze, score, and improve consulting proposal decks automatically.
Upload a .pptx file → Detect sections → Evaluate structure, visuals, and client fit → Get a professional PDF feedback report — all in a few clicks!

## ✨ What It Does?

✅ **Automatic Slide Parsing**
Extracts text from each slide and intelligently maps slides to essential consulting sections like Executive Summary, Problem Statement, Solution Proposal, and Next Steps.

✅ **Structure & Content Validation**
Checks if your proposal has all critical sections and whether the storyline flows naturally.

✅ **Visual Consistency Analysis**
Evaluates fonts, colors, and layouts to ensure your deck looks clean, sharp, and professional.

✅ **Client Fit & Language Scoring**
Assesses if your deck language matches the expected industry standards and the client's tone.

✅ **Multi-Dimensional Scoring**
Generates a weighted overall score combining structure, visuals, and client-fit dimensions.

✅ **Actionable Feedback + PDF Report**
Auto-generates a polished PDF report with personalized improvement tips to make your proposal more impactful.

✅ **Simple Web Interface (Streamlit)**
Just upload your .pptx file and instantly receive a downloadable feedback report!

## 🏗️ Project Architecture
``` bash
consulting_proposal_quality_checker/
├── agents/                     # (Optional) Future agent orchestration (if you want later)
│   └── __init__.py
│
├── schemas/                    # Pydantic models for input/output
│   ├── slide_schema.py
│   └── __init__.py
│
├── services/                   # Business logic / Core services
│   ├── slide_parser.py         # Extract text & titles from slides
│   ├── section_mapper.py       # Map slide titles to consulting sections
│   ├── structure_analyzer.py   # Check if key sections exist
│   ├── visual_analyzer.py      # Check fonts, layouts, design consistency
│   ├── client_fit_analyzer.py  # Analyze language and industry relevance
│   ├── score_aggregator.py     # Multi-dimensional score calculation
│   └── report_generator.py     # PDF feedback generation
│
├── utils/                      # Helper utilities
│   ├── title_detector.py       # Detect titles automatically
│   ├── pdf_utils.py             # Helper to format PDFs
│   └── __init__.py
│
├── streamlit_app/              # Frontend folder
│   ├── app.py                  # Streamlit app
│   └── __init__.py
│
├── outputs/                    # Generated output PDFs
│   └── (Generated reports will be saved here)
│
├── main.py                     # CLI interface to run everything
├── requirements.txt            # Project dependencies
└── README.md                   # Project documentation

```

## 🛠️ Built With-

- Python 3.10+
- Pydantic V2 (for data modeling)
- python-pptx (for slide parsing)
- FPDF (for PDF generation)
- Streamlit (for the web UI)

## ⚡Getting Started-

1. Clone this repo

```bash
git clone https://github.com/<your-username>/consulting-proposal-quality-checker.git
cd consulting-proposal-quality-checker
```
2. Install the dependencies

```bash
pip install -r requirements.txt

```
3. Launch the application

```bash
python main.py
```

4. Web Interface Mode

```bash
streamlit run streamlit_app/app.py
```

## 📄 License
This project is licensed under the MIT License — feel free to use, fork, and improve it!

## 🙌 Why Use This?
In consulting, presentation is everything.
This tool helps ensure your proposals are structured, client-centric, and visually consistent — giving you a competitive edge, and saving hours of manual checking.

### "Good proposals win deals. Great proposals build long-term clients."