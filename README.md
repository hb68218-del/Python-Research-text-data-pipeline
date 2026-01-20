# Research Text Data Processing Pipeline (Python)

**Technical Research & Data Engineering Project**  
**Contributor:** Haeun (Sally) Bae

---

## Introduction

This repository documents my technical contributions to an academic research project involving large scale analysis of unstructured text data. My work focused on designing and implementing a Python based data processing pipeline that converts raw document exports into clean, structured, and analysis ready datasets.

The project emphasizes automation, reproducibility, and data quality. All work presented here reflects **methods and technical implementation only** and does not include unpublished research findings or substantive analysis.

---

## Project Purpose

The purpose of this project was to support academic research by improving how large volumes of unstructured document data are prepared for analysis. Manual document review is inefficient and inconsistent at scale. This pipeline enables systematic, repeatable preprocessing that supports downstream quantitative and qualitative research workflows.

---

## What I Built
<img width="1879" height="761" alt="image" src="https://github.com/user-attachments/assets/c73fb58d-afa3-4bb4-bca0-1665961ed6b8" />
<img width="2279" height="1064" alt="image" src="https://github.com/user-attachments/assets/143f5616-c5e2-42bc-955c-fa5abbafe5bb" />


I designed and implemented an end to end Python pipeline that:

- Ingests large batches of unstructured document files  
- Converts rich text documents into normalized plain text  
- Splits bundled files into individual document level records  
- Extracts structured metadata using pattern matching  
- Applies keyword based flagging to support document filtering  
- Produces clean outputs suitable for research use  

---

## Technical Process Overview

### Document Ingestion
- Automated traversal of raw data directories  
- Preservation of original files for traceability
- <img width="1535" height="904" alt="image" src="https://github.com/user-attachments/assets/58912fc1-e707-47f7-a660-aedb76cc9b3f" />
<img width="836" height="1116" alt="image" src="https://github.com/user-attachments/assets/796f45e6-9b44-47db-9acd-6d79cde209c0" />

### Text Cleaning and Normalization
- Removal of formatting artifacts  
- Standardization of whitespace and encoding  
- Preparation of text for structured parsing
  <img width="1215" height="636" alt="image" src="https://github.com/user-attachments/assets/17b23be2-43c8-484b-90e5-777d2dd51286" />
  <img width="1394" height="830" alt="image" src="https://github.com/user-attachments/assets/cb951e9d-8e1b-4738-9d5b-b45ab789e1a0" />



### Document Segmentation
- Identification of document boundaries within batch files  
- Enforcement of one document per observation
  <img width="859" height="439" alt="image" src="https://github.com/user-attachments/assets/1d5d66ed-1efc-4f43-a85f-2c8e529db9cf" />


### Metadata Extraction
Extracted and standardized fields include:
- Document ID  
- Title  
- Publication date  
- Author  
- Source  
- Firm or organization reference  
- Full document text
<img width="1271" height="985" alt="image" src="https://github.com/user-attachments/assets/c0d67d39-1623-4ca2-a875-9e7d44329769" />


Parsing logic was implemented using regular expressions with fallback rules to reduce missing values.

### Keyword Detection
- Configurable keyword framework  
- Automated scanning across full text  
- Generation of keyword hit counts and indicator flags
  <img width="1526" height="1096" alt="image" src="https://github.com/user-attachments/assets/7a0c4537-aa11-4225-8951-f8dd8380a15f" />


---

## Tools and Technologies Used

- Python  
- Regular expressions  
- CSV and text based data pipelines  
- File system automation  
- Cursor and other GenAI coding assistant

---

## Skills Demonstrated

- Unstructured text processing  
- Python scripting and automation  
- Data cleaning and preprocessing  
- Metadata design and extraction  
- Pipeline development for research workflows  
- Reproducible and auditable data preparation  

---

## Outcome and Impact

The completed pipeline successfully transformed large scale unstructured document exports into structured datasets that could be reliably used by the research team. The technical rigor and scalability of this work contributed to the project being selected for presentation at the **Terry College of Business Annual Stakeholder Research Meeting**, where the focus was on methodology and technical approach.

---

## Notes

This repository presents technical methods only. Research findings, interpretations, and datasets are intentionally excluded to respect ongoing academic work.
