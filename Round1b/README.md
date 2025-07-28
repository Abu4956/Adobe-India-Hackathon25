# 🔍 Adobe India Hackathon 2025 – Round 1B  
## 🤖 Persona-Driven Document Intelligence

This solution extracts and ranks the most relevant sections and sub-sections from a collection of PDF documents based on a **given persona** and their **job-to-be-done**.

---

## 📌 Objective

Given:
- A set of PDF files (3–10)
- A persona (e.g., student, researcher)
- A job to be done (e.g., summarize, extract key concepts)

🎯 Output: A structured JSON highlighting relevant sections and sub-sections from all PDFs, ranked by relevance.

---

## 📂 Input Format

- A folder containing PDF documents (`/app/input`)
- Persona and job should be passed as environment variables (defaults also supported)

### Example:
```bash
PERSONA="PhD Researcher in Computational Biology"
JOB="Prepare a literature review on GNNs for drug discovery"
