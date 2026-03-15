# P-APED: Prompt-based Arabic Phishing Email Dataset

## 📝 Description
**P-APED** is a specialized dataset developed for the detection of Arabic phishing emails, specifically targeting the linguistic and contextual nuances of the MENA region . 

The dataset was constructed using a hybrid approach: collecting raw data and leveraging Large Language Models (**Gemini 2.5 Pro**) via prompt engineering to generate and refine sophisticated phishing scenarios. This ensures that the dataset covers modern attack vectors such as local banking fraud, logistics impersonation, and corporate phishing.


## 📂 Data Structure
| Column | Description |
| :--- | :--- |
| `original_id` | Unique identifier for each entry. |
| `label` | Target class (`Safe Email` or `Phishing Email`). |
| `sector` | The organizational context of the email (e.g., Government, Corporate). |
| `trait` | The psychological personality trait targeted or reflected in the email text. |
| `subject_ar` | The Arabic subject line. |
| `body_ar` | The full Arabic body content of the email. |




