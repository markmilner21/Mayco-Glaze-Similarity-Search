# 🎨 Mayco Glaze Similarity Search

This project builds a **visual similarity search system for ceramic glazes**.

> Given an input image, it returns the most visually similar **Mayco glaze(s)** based on colour, texture, and pattern.

---

## 🚀 Overview

**Pipeline:**

```
PDF documents
    ↓
Image extraction (glaze swatches)
    ↓
Filtering + cleaning
    ↓
CLIP embeddings
    ↓
FAISS index
    ↓
Query image → similar glazes
```

---

## 📁 Project Structure

```
.
├── src/
│   ├── data/
│   ├── features/
│   ├── search/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── report/
├── requirements.txt
└── README.md
```

---

## 📚 Report

All project work is in:

```
report/
```

### Reading order:

- `01-Introduction.ipynb`
- `02-DataSearch.ipynb`
- `03-EDA.ipynb`
- `04-clip.ipynb`
- `05-similarity-search.ipynb`
- `07-Conclusion.ipynb`

---

---

## 🧪 Usage

1. **Extract glaze images**  
   → `03-EDA.ipynb`

2. **Generate embeddings (CLIP)**  
   → `04-clip.ipynb`

3. **Run similarity search (FAISS)**  
   → `05-similarity-search.ipynb`

### Query flow:

```
image → embedding → FAISS → similar images
```

---

## 🧠 Tech Stack

- CLIP (image embeddings)
- FAISS (similarity search)
- OpenCV (image processing)
- PyMuPDF (PDF extraction)
- PyTorch

---

## ⚠️ Limitations

- Not trained specifically on ceramic glazes
- Sensitive to lighting and reflections
- Limited dataset (Mayco-focused)

---

## 🔮 Future Work

- Fine-tune embeddings for glaze-specific features

---

## 📄 Notes

All report content is available in the `report/` folder.

---

## 🙌 Acknowledgements

- Mayco Colors (glaze documentation)
- OpenAI (CLIP)
- Meta AI (FAISS)
