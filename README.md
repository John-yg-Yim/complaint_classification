# 🏛️ Complaint Text Classification and Government Department Recommendation System

This project presents a Korean-language NLP system that automatically classifies civil complaint texts  
into one of **18 predefined categories**.

The final model, based on SKT's KoBERT, achieved high accuracy and reliability.  
A real-time demo is available via Hugging Face Spaces, where users can input a complaint and receive  
both the predicted category and relevant government department contact information.

---

## 📁 Key Files

- **Dataset Source**: [AIHub – AI Language Data for Complaint Handling Automation](https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&dataSetSn=619)

| Filename                       | Description                                      |
|--------------------------------|--------------------------------------------------|
| `complaint_classification.ipynb` | Full experimental pipeline with visualizations  |
| `complaint_classification.html` | Static HTML version (recommended for viewing)   |

> 📝 The trained model is not included,  
> but running the notebook will reproduce the architecture and results.

---

## 🧪 Experiment Summary

- Text preprocessing and duplicate removal (based on `text`, preserving majority `category`)  
- Baseline model using TF-IDF + LightGBM  
- Comparative experiments with KoBERT, RoBERTa, and KcELECTRA  
- Final model selected: **KoBERT with fine-tuning**

---

## 📊 Final Performance Summary (KoBERT)

- **Accuracy**: 93.8%  
- **Macro F1-score**: 92%  
- **Weighted F1-score**: 94%  
- Achieved stable performance across both major and minority classes

---

## 🔗 Dataset Info

- Source: Public Korean civil complaint texts (detailed origin not disclosed)  
- Total 18 categories: e.g., `Transportation`, `Welfare`, `Public Health`, `Automobile`, `Sanitation`, etc.  
- Personally identifiable information removed and categories unified based on central government criteria

---

## 🚀 Demo

- Hugging Face Demo (Real-time text classification + department info)  
👉 [Complaint Classification & Government Department Recommendation](https://huggingface.co/spaces/John-Yim/ProjectNote)
