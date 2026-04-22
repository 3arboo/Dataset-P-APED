# P-APED: Prompt-based Arabic Phishing Email Dataset

## 📝 Overview

**P-APED** is a high-diversity dataset specifically engineered to address the scarcity of realistic Arabic phishing data. While most existing datasets rely on poor machine translations, P-APED utilizes **Gemini 1.5 Pro** and advanced prompt engineering to generate linguistically natural and culturally relevant phishing scenarios targeting the MENA region.

The dataset bridges the gap between traditional social engineering tactics and modern, localized cyber threats, covering sectors like regional banking, government services, and corporate logistics.

-----

## ⚙️ Methodology

The dataset construction follows a rigorous four-stage pipeline to ensure semantic integrity and regional authenticity.

1.  **Baseline Collection:** Extraction of core intent from human-authored English social engineering corpora.
2.  **LLM-Driven Augmentation:** Leveraging **Gemini 2.5 Pro** to refine messages. Unlike standard translation, this process generates content natively in Arabic, incorporating local dialects and cultural nuances.
3.  **Labeling & Classification:** Systematic categorization into `Safe` and `Phishing` classes.
4.  **Aggregation:** Final compilation into a high-diversity corpus designed for training robust NLP detection models.

-----

## 📂 Data Structure

The dataset is structured to support both binary classification and granular behavioral analysis.

| Column | Description |
| :--- | :--- |
| `original_id` | Unique identifier for each entry. |
| `label` | Target class: `Safe Email` or `Phishing Email`. |
| `sector` | Organizational context (e.g., Government, Banking, Corporate). |
| `trait` | Psychological trigger used (e.g., Urgency, Authority, Fear). |
| `subject_ar` | The Arabic subject line. |
| `body_ar` | The full Arabic body content. |


```
