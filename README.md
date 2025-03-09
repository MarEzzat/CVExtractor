# CVExtractor
Extract key information from resumes with ease using BERT and regex-powered parsing.

## Overview

ResumeParserX is a Python-based tool designed to extract essential entities from resume PDFs, including:
- **Name**: The full name of the candidate.
- **Phone**: The candidate’s contact number.
- **Education Location**: The institution where the candidate studied (e.g., university name).
- **Education Year**: The start year of the candidate’s education.

Built with the `transformers` library’s BERT NER model (`dslim/bert-base-NER`) and robust regex fallbacks, this tool handles varying resume formats efficiently.

## Features
- Uses pre-trained BERT for named entity recognition (NER) to identify names and organizations.
- Employs regex for phone numbers and education years, ensuring reliability across diverse layouts.
- Fallback mechanisms to extract entities when BERT tagging is incomplete.
- Outputs results to a clean `resume_entities.txt` file.

## Prerequisites
- Python 3.6+
- Libraries: `pdfplumber`, `transformers`, `torch`
- Google Colab (optional, for easy file upload and execution)

Install dependencies:
```bash
pip install pdfplumber transformers torch

## Google Colab (Notebook link)
[Colab](https://colab.research.google.com/drive/1TPHOcqqqUhQ9MFmOCmswTwYjFbgrV74S?usp=sharing)
