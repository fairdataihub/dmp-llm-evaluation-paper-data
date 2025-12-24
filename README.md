# LLM–NIH DMP Evaluation (Paper 1)

Code and analysis artifacts for **“Evaluating the Performance of LLMs in Creating NIH Data Management Plans.”**  
This repository contains (1) automatic evaluation pipelines and (2) human evaluation analysis used to generate paper results, figures, and tables.

---

## Setup (Recommended)

### 1) Create a virtual environment
```bash
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate
```

### 2) Install dependencies
Automatic evaluation:
```bash
pip install -r DMP_Automatic_Evaluation_Analysis/Requirements.txt
```

Human evaluation:
```bash
pip install -r DMP_Human_Evaluation_Analysis/requirements.txt
```

