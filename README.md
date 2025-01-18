Overview

The Generative AI Resume Analyzer automates resume screening using advanced AI techniques. It extracts key fields from resumes, scores candidates based on AI/ML experience, processes multiple resumes efficiently, and outputs structured results in Excel format.

Features

Resume Parsing: Extracts essential details such as Name, Contact, University, Course, CGPA, and Skills.

AI/ML & Gen AI Scoring: Assigns experience scores based on relevant keywords and context.

Batch Processing: Handles up to 100 resumes at a time for efficient analysis.

Structured Output: Saves extracted information and scores in an Excel file.

Few-Shot Learning: Adapts to different resume formats for better accuracy# Genrative-AI-Powered-Resume-Analyzer-

Requirements

1. Dependencies

Ensure you have the following Python libraries installed:

pip install pdfplumber spacy pandas openpyxl concurrent.futures

Download the necessary NLP model:

python -m spacy download en_core_web_sm

2. Input

A folder named resumes/ containing PDF resumes.

3. Output

An Excel file (resume_analysis.xlsx) containing structured resume data.

Usage

Step 1: Place Resumes in the Folder

Ensure all resumes (PDF format) are stored inside the resumes/ directory.

Step 2: Run the Script

Execute the Python script:

python resume_parser_ai.py

Step 3: View the Results

Once the script completes, check the resume_analysis.xlsx file for extracted details and scores.

Scoring Criteria

Gen AI Experience Score:

1: Exposed (Basic familiarity, coursework exposure)

2: Hands-on (Implemented projects, internships)

3: Advanced (Agentic RAG, evaluations, research)

AI/ML Experience Score:

1: Basic exposure

2: Hands-on implementation

3: Advanced model work (Transformers, Neural Networks)

Code Explanation

The script follows these key steps:

Load Resumes: Reads PDF files from the resumes/ folder using pdfplumber.

Extract Text: Converts the PDF content into raw text for processing.

Parse Key Fields: Uses spaCy NLP for extracting important fields like Name, Contact, University, and Skills.

Scoring System:

Checks for AI/ML-related keywords to assign experience scores.

Uses a predefined dictionary of terms related to AI/ML & Gen AI.

Batch Processing: Utilizes concurrent.futures for handling multiple resumes simultaneously.

Save to Excel: Stores extracted data in resume_analysis.xlsx using pandas and openpyxl.

Future Enhancem
