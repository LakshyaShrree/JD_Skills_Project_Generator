# JD_Skills_Project_Generator

AI-based tool that maps job descriptions to unique project ideas using **Gemini API**

🤖 **AI-Powered Gemini Prompt Generator** (Google Generative AI)  
This Colab notebook uses Google's Generative AI (`google-generativeai`) to generate content via the **Gemini 1.5 Flash** model.

---

## 🛠️ Setup Instructions

### 1. Get Your Gemini API Key
- Visit: [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)  
- Generate an API key from your Google AI Studio account.

---

### 2. Insert Your API Key
📌 Add the following code block **after Cell 2** (i.e., after the library import cell):

```python
import os
os.environ["GEMINI_API_KEY"] = "your-api-key-here"  # 🔑 Replace this with your actual Gemini API key


