# Powerweave
Code Repository for AI-Powered Purchase Order Automation
This repository contains a proof-of-concept (PoC) solution for automating the extraction, transformation, and harmonization of order data from diverse document formats (Excel, PDF, Word, CSV, Scanned forms) into a standardized JSON schema.

The project simulates how an AI-powered pipeline can reduce manual effort, improve accuracy, and streamline integrations with vendor systems.
Problem Statement

Companies receive 500–800 purchase orders per month from 25+ clients in different formats (Excel, PDF, Word, CSV, scanned forms). Processing these manually leads to:

Delays in order handling

Human errors in data entry

Inefficient downstream operations

The goal: automate document parsing + standardize data into a JSON schema for a single vendor.
Proposed Solution (Architecture Overview)

1. Document Ingestion

Upload via portal / email / API

Supports Excel, PDF, Word, CSV, Scanned

2. AI-Powered Extraction

OCR for scanned forms (Tesseract / Azure Form Recognizer / Google Document AI)

NLP + schema mapping (spaCy, HuggingFace models)

3. Transformation & Harmonization

Cleaning, validation, date normalization

Mapping custom fields → unified JSON schema

4. Output

Standard JSON file ready for vendor integration

Confidence score + error handling

Human-in-the-loop for low-confidence cases

Tech Stack
MVP (Proof of Concept)

Python (pandas, openpyxl) → Excel parsing

json module → JSON schema generation

Pymupdf

Jupyter Notebooks → quick experimentation
