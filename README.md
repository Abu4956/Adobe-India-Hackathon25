Absolutely! Here's a clean, professional, and complete `README.md` for your **entire project repository** — combining both **Round 1A** and **Round 1B** of the **Adobe India Hackathon 2025**.

---

## ✅ `README.md` for Root of Repository

````markdown
# 📘 Adobe India Hackathon 2025 – "Connecting the Dots"

Welcome to my submission for the Adobe India Hackathon 2025!  
This project reimagines how we read and interact with PDFs — turning them into intelligent, structured, and personalized experiences.

---

## 🧠 Problem Statement

**Challenge Theme**: *Connecting the Dots Through Docs*

We were asked to reimagine the humble PDF as a smart, structured, and responsive experience. The hackathon was divided into two rounds:

---

## 📍 Round 1A – Structured Outline Extraction

🔎 **Goal**: Extract a clean, hierarchical outline from any PDF including:

- Document **Title**
- Headings: **H1**, **H2**, **H3**
- Page numbers

📂 Folder: `round1a/`

### ✅ Features:
- Uses **PyMuPDF** for layout-aware parsing
- Clusters font sizes with **KMeans** to identify heading levels
- Outputs valid JSON in the required format

### 📤 Sample Output:
```json
{
  "title": "Understanding AI",
  "outline": [
    { "level": "H1", "text": "Introduction", "page": 1 },
    { "level": "H2", "text": "What is AI?", "page": 2 }
  ]
}
````

📦 Fully Dockerized and offline, with execution time ≤ 10s on 50-page PDFs

---

## 📍 Round 1B – Persona-Driven Document Intelligence

🧑‍💼 **Goal**: Extract and prioritize the most relevant sections from a collection of PDFs based on:

* A given **persona**
* Their **job to be done**

📂 Folder: `round1b/`

### ✅ Features:

* Embeds PDF chunks and persona intent using **Sentence Transformers**
* Computes **cosine similarity** to rank content
* Outputs structured JSON with both **section summaries** and **detailed sub-sections**

### 🧠 Use Case Example:

> Persona: *PhD Researcher in Computational Biology*
> Job: *Prepare a literature review on GNNs for drug discovery*

### 📤 Output Includes:

* Metadata (persona, job, docs)
* Top matching sections (titles + pages)
* Most relevant text chunks

📦 Runs completely offline, CPU-only, with <100MB model size and ≤60s processing time.

---

## 🧰 Tech Stack

| Component        | Tools Used                           |
| ---------------- | ------------------------------------ |
| PDF Parsing      | PyMuPDF                              |
| Clustering (1A)  | scikit-learn (KMeans)                |
| Embeddings (1B)  | Sentence Transformers (MiniLM-L6-v2) |
| Containerization | Docker                               |
| Language         | Python 3.10                          |

---

## 🐳 How to Run

Each round is inside its own folder (`round1a/` and `round1b/`) with:

* `main.py`
* `Dockerfile`
* `requirements.txt`
* `README.md`
* `approach_explanation.md`

See their README files for specific build/run commands.

---

## 📁 Project Structure

```
📂 Adobe-India-Hackathon25/
├── round1a/                   # Round 1A: Outline extractor
│   ├── main.py
│   ├── Dockerfile
│   ├── README.md
│   ├── requirements.txt
│   └── approach_explanation.md
│
├── round1b/                   # Round 1B: Persona-driven intelligence
│   ├── main.py
│   ├── Dockerfile
│   ├── README.md
│   ├── requirements.txt
│   └── approach_explanation.md
│
└── README.md                  # ← This file (overall project README)
```

---

## 📌 Constraints Met

| Requirement                  | Status ✅ |
| ---------------------------- | -------- |
| Offline Execution            | ✅        |
| CPU-only (no GPU)            | ✅        |
| Model Size Limits (≤1GB)     | ✅        |
| Time Limits (10s / 60s)      | ✅        |
| No hardcoding or assumptions | ✅        |

---

## 👤 Author

**Abu Obaida**
GitHub: [@Abu4956](https://github.com/Abu4956)

---

🎯 Thank you Adobe for this exciting opportunity to reimagine how we read, learn, and connect through documents!

```

---

Let me know if you'd like a `LICENSE`, GitHub badges, or help polishing the presentation for final submission.
```
