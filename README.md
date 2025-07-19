# 📌 Job Insight Clustering for Proactive Prompt Engineering Goal

A prototype pipeline for generating structured job insights and clustering career trajectories, designed to support agentic AI-based **Proactive Job Goal Creation**. This repository includes extraction scripts, embedding workflows, and clustering logic, enabling insight generation from real-world Japanese job postings (PDF format).

---

## 🧠 Project Purpose

This Minimum Viable Product(MVP) explores a scalable method to identify latent career goal patterns—especially around the *Prompt Engineering* domain—by:

- Extracting structured data from unstructured job PDFs
- Encoding semantic job representations via SentenceTransformer
- Clustering embeddings to reveal role-level segmentation and insights
- Visualizing outcomes for human-readable career guidance

---

## 📁 Repository Structure

```
├── input_pdfs/               # Job posting PDFs collected via keyword search (collect one-self current web opened information)
├── output_jsons/             # Structured JSON files per job posting
├── embeddingtxt_clusteringkm_tsnev1.ipynb     # Natural text generation & embedding extraction, Dimensionality reduction & cluster labeling
├── cluster_visualizer_positionchartv1.ipynb        # pie chart & 2D projection of job embedding space
├── clustering_results.csv    # Final summary table of 161 samples
├── tsne_visualization_data.csv    # 2D scores via dimensionality reduction
├── ai_job_market_distribution.png    # Pie chart : Prompt engineer position insight 
├── cluster_tsne_plot.png    # t-SNE plot : clustered positions on job embedding space
└── README.md                 # Project overview and instructions
```

---

## ⚙️ Key Technologies

- `pdfplumber`, `pandas`: For data extraction & manipulation
- `gpt-4o-mini-2024-07-18`: Summarize job posting text into position, industory, job description, size of workforce, and established year
- `sentence-transformers`: Multilingual semantic embedding  
- `scikit-learn`: Clustering algorithms (KMeans, t-SNE)  
- `matplotlib`: Role distribution & embedding space visualization

---

## 📊 Clustering Summary (N=161)

| Cluster | Label                              | Count | Description |
|---------|------------------------------------|-------|-------------|
| 0       | Generative AI Implementation       | 92    | Engineering & Applied AI professionals |
| 1       | AI Strategy & Business Design      | 43    | Management, strategy, and applied planning roles |
| 2       | Advanced AI R&D Engineers          | 26    | Research-focused, LLM/NLP development roles |

Visualizations include:
- Pie chart showing cluster distribution
- t-SNE plot highlighting semantic separability

---

## 🚀 Future Directions

- Job goal recommendation powered by Agentic AI  
- Cross-domain comparison (e.g. by industry, company size, maturity)  
- Integration into candidate-facing career mapping tools  
- Dynamic labeling of emerging roles via continual learning

---

## 📬 Author

Crafted by Takato – AI/ML Engineer & Strategic Technologist  
Focused on long-term impact at the intersection of agentic systems and societal value.
LinkedIn: https://www.linkedin.com/feed/update/urn:li:activity:7352022495954169857/

---

## 📝 License

MIT License / Please cite appropriately when using job clustering insights.

```
