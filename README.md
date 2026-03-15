# P-APED: Prompt-based Arabic Phishing Email Dataset

## 📝 Description
**P-APED** is a specialized dataset developed for the detection of Arabic phishing emails, specifically targeting the linguistic and contextual nuances of the MENA region (including the Algerian dialect/context). 

The dataset was constructed using a hybrid approach: collecting raw data and leveraging Large Language Models (**Gemini 2.5 Pro**) via prompt engineering to generate and refine sophisticated phishing scenarios. This ensures that the dataset covers modern attack vectors such as local banking fraud, logistics impersonation, and corporate phishing.

## 📊 Dataset Specifications
- **Name:** P-APED (Prompt-based Arabic Phishing Email Dataset)
- **Total Samples:** 672
- **Balance:** Perfectly Balanced (50% Safe / 50% Phishing)
- **Samples per Class:** 336 Safe Emails, 336 Phishing Emails
- **Language:** Arabic (Modern Standard & Dialectal influences)
- **Format:** CSV

## 📂 Data Structure
The dataset contains the following key columns:
| Column | Description |
| :--- | :--- |
| `subject_ar` | The subject line of the email in Arabic. |
| `body_ar` | The main content/body of the email. |
| `text` | The combined text (Subject + [SEP] + Body) used for Transformer training. |
| `label` | Categorical label (`Safe Email` or `Phishing Email`). |
| `label_num` | Numerical label (0 for Safe, 1 for Phishing). |

## 🛠 Methodology
1. **Data Collection:** Gathering authentic Arabic email templates.
2. **LLM Augmentation:** Using Gemini 2.5 Pro to generate diverse phishing variants based on real-world prompts.
3. **Preprocessing:** Merging features and cleaning text.
4. **Balancing:** Applied **Random Undersampling** on the "Safe" class to match the "Phishing" class count to eliminate model bias.

## 🚀 Benchmarking Results
This dataset has been benchmarked using various architectures:
- **MarBERT:** 98.02% Accuracy
- **Ensemble Stacking:** 97.03% Accuracy
- **CNN (1D):** 96.30% Accuracy
- **XGBoost:** 93.58% Accuracy


