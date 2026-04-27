# Receipt-Data-Extraction-Analysis-System
This project extracts structured data from receipt images using OCR and post-processing techniques. It identifies key fields such as **store name**, **date**, and **total amount**, and outputs them in a clean JSON format. The system is designed to handle noisy, inconsistent, and low-quality receipt data.

## 🧠 Problem Statement
Receipt data extraction is challenging due to:
- Variability in formats and layouts
- OCR noise and misclassification
- Missing or ambiguous fields (especially totals and dates)

This project builds a pipeline to clean, structure, and evaluate extracted data using confidence scores.

## 📂 Project Structure
- Carbon_crunch_Assignment.ipynb → Main processing notebook  
- results.json → Extracted structured output  
- images/ → Input receipt images  

## ⚙️ Features
- OCR-based text extraction  
- Data cleaning & normalization  
- Confidence scoring for each field  
- Structured JSON output  
- Graceful handling of missing/low-confidence values  

## 📊 Sample Output
json
{
  "store_name": { "value": "WHOLE FOODS", "confidence": 0.98 },
  "date": { "value": "9/15/2020", "confidence": 0.85 },
  "total_amount": { "value": "28.28", "confidence": 0.62 }
}
