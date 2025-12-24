# LLM–NIH DMP Evaluation (Paper 1)

Code and analysis artifacts for **“Evaluating the Performance of LLMs in Creating NIH Data Management Plans.”**  
This repository contains (1) automatic evaluation pipelines and (2) human evaluation analysis used to generate paper results, figures, and tables.

---
## Repository Structure

```
LLM-NIH-DMP-EVALUATION/
├─ DMP_Automatic_Evaluation_Analysis/
│  ├─ inputs/                       # Input DMPs / reference samples / configs (notebooks read from here)
│  ├─ outputs/                      # Generated metrics, intermediate files, result tables
│  ├─ Approach-new version-DMP.ipynb# Main notebook for automatic evaluation (ROUGE/SBERT/etc.)
│  ├─ Requirements.txt              # Python dependencies for automatic evaluation
│  ├─ .env                          # Local environment variables (DO NOT commit)
│  └─ .gitignore
│
└─ DMP_Human_Evaluation_Analysis/
   ├─ Clean DMP/                    # Cleaned/standardized DMP text for review and analysis
   ├─ data/                         # Survey exports, reviewer labels, mapping files
   ├─ plots/                        # Final figures for the manuscript
   ├─ Survey.ipynb                  # Survey processing and summary stats (if separated)
   ├─ requirements.txt              # Python dependencies for human evaluation analysis
   ├─ .env                          # Local environment variables (DO NOT commit)
   └─ .gitignore
```

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

