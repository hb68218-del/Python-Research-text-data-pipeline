

# Python-Research-text-data-pipeline

## Project Objective

This project examines instances of government retaliation against publicly traded firms using large scale news and document data. The objective is to transform unstructured document exports into structured, analysis ready datasets that support content analysis, interrater reliability testing, and empirical research.

The project progresses from raw document ingestion to automated parsing, metadata extraction, keyword classification, and data validation. Emphasis is placed on reproducibility, scalability, and methodological transparency.

---

## Problem Overview

Large scale research on government firm interactions requires systematic identification of relevant events across thousands of documents. Manual review is time intensive, difficult to replicate, and prone to inconsistency.

This project addresses these challenges by implementing an automated data processing pipeline that standardizes document handling and classification.

---

## Tools and Technologies Used

- Python for text processing and automation 
- Regular expressions for structured parsing  
- CSV and plain text data pipelines
- Cursor and other genAI coding assistant

---

## Data Description

### Data Sources

- Factiva news exports  
- Batch `.rtf` files containing multiple articles per file
<img width="1535" height="904" alt="image" src="https://github.com/user-attachments/assets/58912fc1-e707-47f7-a660-aedb76cc9b3f" />
<img width="836" height="1116" alt="image" src="https://github.com/user-attachments/assets/796f45e6-9b44-47db-9acd-6d79cde209c0" />


### Data Scope

- Publicly traded firms  
- Coverage across multiple U.S. states  
- Multi year time span  

---

## Data Processing Pipeline

### File Ingestion

- Imported raw document exports in batch format  
- Preserved original files in read only state  
- Automated directory traversal for scalable processing



### Text Conversion and Cleaning

- Converted rich text documents to plain text  
- Removed formatting artifacts and encoding inconsistencies  
- Standardized whitespace and line breaks

### Document Segmentation

- Identified article boundaries within bundled files  
- Split batch files into individual documents  
- Ensured one document per observation  

---

## Metadata Extraction

### Metadata Fields Extracted

- Document ID  
- Title  
- Publication date  
- Author  
- Source  
- Firm or organization reference  
- Full article text  
<img width="1587" height="1225" alt="image" src="https://github.com/user-attachments/assets/24dcc8ed-b881-4f17-aa24-fd6ffd30aede" />

### Extraction Logic

Metadata was extracted using structured pattern matching and fallback rules to minimize missing values and ensure consistency across documents.

---

## Keyword Classification and Topic Tagging

### Keyword Framework
<img width="1528" height="1094" alt="image" src="https://github.com/user-attachments/assets/6cdf163d-a576-440f-a5da-69d740ecf0da" />

- Government actions and enforcement  
- Regulatory and legal disputes  
- Public policy responses  
- Firm level reactions  

### Classification Method

- Automated keyword detection across full document text  
- Generated keyword hit counts per document  
- Assigned categorical flags for downstream analysis  
- Logged ambiguous cases for manual review  

---

## Data Validation and Quality Control
<img width="2232" height="813" alt="image" src="https://github.com/user-attachments/assets/3f044252-c233-4419-97ec-8e09ca802dd6" />

### Structural Validation

- Verified one row per document  
- Confirmed alignment between metadata and text outputs  

### Content Validation

- Flagged incomplete or low confidence documents  
- Logged cases requiring additional review  

---

## Research Outputs

### Structured Outputs

- Metadata dataset in CSV format  
- Cleaned document level text files  


### Analytical Outputs

- Summary metrics on document coverage  
- Keyword frequency distributions  
<img width="1879" height="761" alt="image" src="https://github.com/user-attachments/assets/c73fb58d-afa3-4bb4-bca0-1665961ed6b8" />

---

## Limitations

### Methodological Limitations

- Keyword based classification may produce false positives  
- Context dependent interpretation required  

### Data Limitations

- Coverage limited to available news reporting  
- Variation in document structure across sources  

---
## Technical Skills Demonstrated

- Python scripting and automation  
- Text processing and regular expressions  
- Data cleaning and preprocessing  
- Pipeline design for unstructured data  
- Reproducible research workflows  
- Data validation and quality control  

---

## Outcome and Impact

The technical pipeline successfully transformed large scale unstructured document exports into clean, structured datasets suitable for academic research workflows. The reliability, scalability, and clarity of the technical implementation contributed to the project’s selection for presentation at the **Terry College of Business Annual Stakeholder Research Meeting**, where the focus was on methodology and technical approach rather than research findings.
