# Data Cleaning Assistant (with Gradio + NLP)

An interactive Gradio application that allows users to upload a CSV file and perform data cleaning operations using natural language commands. Results can be downloaded or saved directly to an SQLite database.

> Powered by `pandas`, `Gradio`, `SQLAlchemy`, and a custom NLP parser for hands-free data wrangling.

---

## 🗂Files Included

| File              | Purpose                                                       |
|-------------------|---------------------------------------------------------------|
| `app.py`          | Main Gradio UI app to handle user input and show outputs      |
| `cleaning_utils.py` | Core cleaning logic (e.g., drop NA, convert types, outlier removal) |
| `nlp_parser.py`   | NLP rule-based parser to convert user commands to actions     |
| `db_loader.py`    | Handles SQLite export via SQLAlchemy                          |
| `requirements.txt`| List of dependencies                                          |
| `Pipfile`         | Optional: alternative dependency manager                      |
| `.gitignore`      | Ignores `.env`, cache, etc.                                   |
| `.env.example`    | (Optional) Example of any sensitive config you might need     |

---

## Features

- Upload and clean any CSV file via a simple UI
- Use plain English to run cleaning tasks:
  - `drop missing`, `fill missing`, `drop duplicates`, etc.
- Preview or save the cleaned data to a SQLite DB
- Download cleaned results as CSV
- Browser-based — runs locally with auto-launch

---

## Supported Commands

Type these in the chat interface after uploading a dataset:

- `drop missing`
- `fill missing`
- `drop duplicates`
- `standardize column names`
- `convert age to int`
- `remove outliers from salary`
- `rename column old_name to new_name`
- `drop column unnecessary_column`
- `load to sql`

---

