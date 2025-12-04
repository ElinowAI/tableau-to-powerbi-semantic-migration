✅ README.md – version prête pour GitHub

(tu peux copier/coller dès que tu confirmes le nom du repo)

🟣 Tableau → Power BI Semantic Model Migration
Automated framework to translate Tableau formulas, metadata & semantic structure into Power BI

This repository provides an open, modular architecture to automatically migrate semantic content from Tableau to Power BI:

✔ Extract Tableau metadata

Using GraphQL API with Personal Access Token (PAT):

Workbooks

Data sources

Fields

Calculated fields

Relationships

Data roles / data types

✔ Translate Tableau formulas into DAX

Full formula parser

Syntax tree

Function mapping (e.g. ZN() → COALESCE(), WINDOW_SUM() → CALCULATE() patterns)

Error handling & unsupported patterns detection

✔ Generate Power BI Semantic Model

Measures

Columns

Hierarchies

Relationships

Model JSON export (PBIM / Tabular Editor compatible)

📐 Architecture
🔹 1. Tableau GraphQL Layer

Extract metadata via PAT authentication.

🔹 2. Translation Engine

Tableau formula parser

Function mapping rules

DAX generator

AST transformation

🔹 3. Semantic Model Builder

Generates a Power BI model definition JSON.

🔹 4. Output

✔ DAX measures
✔ Tables & relationships
✔ Full semantic model
✔ Documentation for migration
