# Quantifying Narrative Surprise

This project develops NLP methods to detect and measure **plot twists** in thriller short stories, framing **narrative surprise** as a sequential anomaly detection task. By combining **probabilistic models (surprisal-based)** and **embedding-based models (semantic shift)**, we provide a computational framework for quantifying suspense in narrative texts.

---

## 📌 Project Goals
- Formalize **suspense** and **plot twists** within an NLP framework.  
- Quantify twist magnitude using **probabilistic divergence** and **semantic deviation**.  
- Analyze thriller stories to study narrative structure and build **twist-based ranking systems**.  

---

## 🧩 Methodology
1. **Expectation Modeling** – Use language models to estimate narrative progression.  
2. **Twist Detection** – Identify narrative units that diverge significantly from expectations.  
3. **Scoring** – Assign quantitative **twist scores** based on surprisal or embedding shifts.  
4. **Corpus-Level Analysis** – Aggregate twist scores to visualize suspense trajectories across stories.  

---

## 📊 Data
- **Sources**: Thriller short stories from [Reedsy Prompts](https://blog.reedsy.com/short-stories/thriller/) and [Short Fiction Break](https://shortfictionbreak.com/category/genre/thrillersuspense/).  
- ~100 stories, 200–250 sentences each (≈270k words total).  

---

## ✅ Evaluation
- **Event-level**: Precision, recall, F1-score against manually annotated twists.  
- **Corpus-level**: Correlation with human judgments of suspense.  
- **Baselines**: Random labeling and heuristic (rare words/long sentences).  

---

## 🔍 Applications
- **Computational literary studies** – Formalizing narrative surprise.  
- **Creative AI** – Generating and analyzing engaging storylines.  
- **Cultural analytics** – Large-scale studies of suspense in fiction.  

---

## 🚀 Work Plan
1. Data acquisition & preprocessing  
2. Formal task definition  
3. Model implementation & training  
4. Evaluation & validation  
5. Analysis & visualization  

---

## 📖 References
- Levy, R. (2008). *Expectation-based syntactic comprehension.* Cognition.  
- Piper, A., Xu, H., & Kolaczyk, E. (2023). *Modeling narrative revelation.* CHR 2023.  
- Wilmot, D. & Keller, F. (2020). *Modeling suspense in short stories.* ACL.  
- Underwood, T. (2024). *Can language models predict the next twist in a story?*  

---

## 👥 Team
- **Devashish Juyal** – Department of EECS, University of Michigan  
- **Yuganshi Agrawal** – Department of Statistics, University of Michigan  

---

## ⚡ Quick Start
```bash
# Clone repository
git clone https://github.com/<your-username>/narrative-surprise.git
cd narrative-surprise

# Install dependencies
pip install -r requirements.txt

# Run preprocessing
python scripts/preprocess.py --data data/

# Train model
python scripts/train.py --config configs/surprisal.yaml
