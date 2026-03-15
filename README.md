# P-APED: Prompt-based Arabic Phishing Email Dataset

## 📝 Description
**P-APED** is a specialized dataset developed for the detection of Arabic phishing emails, specifically targeting the linguistic and contextual nuances of the MENA region . 

The dataset was constructed using a hybrid approach: collecting raw data and leveraging Large Language Models (**Gemini 2.5 Pro**) via prompt engineering to generate and refine sophisticated phishing scenarios. This ensures that the dataset covers modern attack vectors such as local banking fraud, logistics impersonation, and corporate phishing.


## 📂 Data Structure
The dataset contains the following key columns:
| Column | Description |
| :--- | :--- |
| `subject_ar` | The subject line of the email in Arabic. |
| `body_ar` | The main content/body of the email. |
| `label` | Categorical label (`Safe Email` or `Phishing Email`). |





