# Data Cleaning Assistant (Gradio App)

A conversational Gradio app for quick, no-code data cleaning of CSV files.  
Upload your dataset, type a natural-language cleaning command, and see instant results.

## Features

- **Natural Language Command Parsing** (e.g., “drop missing”, “convert age to int”)
- **CSV Upload and Cleaning** using common pandas transformations
- **NLP Parser** for mapping chat commands to Python actions
- Built-in actions:
  - Drop missing/duplicate values
  - Fill missing values
  - Standardize column names
  - Convert column types
  - Remove outliers (Z-score)
  - Rename/drop columns
- **SQLite Database Export** using SQLAlchemy
- Download cleaned CSV
- SQL Table Preview (Markdown format)



