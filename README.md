# JD_Skills_Project_Generator

AI-based tool that maps job descriptions to unique project ideas using **Gemini API**

🤖 **AI-Powered Gemini Prompt Generator** (Google Generative AI)  
This Colab notebook uses Google's Generative AI (`google-generativeai`) to generate content via the **Gemini 1.5 Flash** model.

---

## 🛠️ Setup Instructions

🔐 API Key Setup Instructions
This project uses the Gemini 1.5 Flash model from Google’s Generative AI suite. To use it, you’ll need a Gemini API key.

You can get one from:
👉 https://aistudio.google.com/app/apikey

✅ For Google Colab Users (Recommended)
No API key is stored in the code. You must use the Colab Secrets Manager:

Open the notebook in Google Colab.

On the left sidebar, click the 🔑 Secrets tab.

Click “+ Add a new secret”

Set:

Name: GOOGLE_API_KEY

Value: (Paste your Gemini API key here — starts with AI.....)

Run the notebook — it will fetch the key securely via:

from google.colab import userdata
GOOGLE_API_KEY = userdata.get('GOOGLE_API_KEY')

This approach keeps your key hidden and allows safe GitHub sharing.

🖥️ For VS Code / Local Python Users
If you're running this notebook or script locally (e.g., in VS Code, Jupyter, etc.), follow these steps:

In your terminal, export the API key:

Linux/macOS:export GEMINI_API_KEY=your-api-key-here
Windows (CMD):set GEMINI_API_KEY=your-api-key-here

Or set it in Python before configuring Gemini:
import os
os.environ["GEMINI_API_KEY"] = "your-api-key-here"

Then configure the API:

import google.generativeai as genai
genai.configure(api_key=os.getenv("GEMINI_API_KEY"))

This keeps the key outside your code and protects it when sharing.

🔒 Security Notes (Safe for GitHub)
✅ API key is stored using Colab Secrets Manager

✅ Key is not hardcoded or printed in the notebook

✅ This ensures the notebook is safe to upload publicly to GitHub

✅ Users are instructed to add their own API key before use


 
