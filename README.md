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


## 🤔 Why Build This When ChatGPT or Gemini Can Do It Directly?

You're absolutely right — technically, yes, you could open ChatGPT or Gemini and ask:

> “Suggest a project for an Amazon data engineer job”

But here's why this tool is still valuable and needed:

---

### 💡 Why This Project Is Needed Despite ChatGPT

#### 🔹 1. Automation + Repeatability
- Automates the prompt logic  
- Provides consistent, structured, and repeatable output  
- No need to rephrase manually every time  

💬 ChatGPT ≠ reusable pipeline  
🧠 This tool = a repeatable project recommender framework

---

#### 🔹 2. User Personalization
- Allows users to select skill level (Beginner / Intermediate / Advanced)  
- Tailors project suggestions accordingly  

Manual prompts in ChatGPT would require tweaking every time. This tool builds that logic in.

---

#### 🔹 3. Job Description Parsing
- Takes a real job description  
- Extracts the core skills  
- Generates project ideas + learning resources  

🔁 Structured mapping: **JD → Skills → Projects**

---

#### 🔹 4. Student-Friendly, Guided Experience
- No prompt engineering expertise required  
- Paste a JD, select a level, click Run — that’s it  
- Output includes:
  - ✅ Extracted skills  
  - ✅ 3 smart projects  
  - ✅ Learning links  
  - ✅ Time estimates  

💡 It becomes a self-serve **AI career mentor**, not just a chat.

---

#### 🔹 5. GitHub-Integrated, Reusable Tool
This isn't just a one-time ChatGPT session.  
It's a **working notebook** that can be cloned, reused, and extended.

