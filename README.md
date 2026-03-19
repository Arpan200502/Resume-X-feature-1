  # 🧠 AI Resume Builder  

**ATS-Optimized • One-Page • AI-Powered** 
   
An **AI-powered resume builder** that generates **ATS-friendly, one-page resumes** using modern Large Language Models (LLMs).

The app takes **unstructured user input** (education, experience, projects, skills) and converts it into **professionally written, print-ready resumes** using multiple templates.

> 👉 **No backend required** — users securely provide **their own API key**.  
 
---

  
## ✨ Key Features 
### 🧾 One-Page A4 Resume Enforcement

* Automatically fits content into **exactly one A4 page**
* **Smart compact mode** for longer resumes
* No overflow, no scrolling

---

### 🤖 AI-Generated Content

* Converts raw notes into **achievement-driven bullet points**
* Adds **quantified impact** (percentages, metrics, improvements)
* Uses **ATS-optimized wording and structure**

---

### 🎨 Multiple Resume Templates

* **Modern**
* **ATS Classic (Serif)**
* **Dark Sidebar**
* **Minimal / Olivia-style**

---

### 🔐 User-Provided API Key

* No hard-coded API keys
* Users enter their own **Groq / Cohere / compatible LLM API key**
* API key stored **locally** using `localStorage`

---

### 🖨️ Print-Perfect PDF Export

* Resume rendered inside an **iframe**
* Browser print → **pixel-perfect A4 PDF**
* Colors, fonts, and layout preserved

---

### ⚡ Frontend-Only

* Pure **HTML, CSS, and JavaScript**
* No server
* No database
* No authentication required

---

## 🧑‍💻 Tech Stack

### Frontend

* **HTML5**
* **CSS3** (custom, no framework)
* **Vanilla JavaScript**

### AI / LLM APIs

* **Groq API** (LLaMA-3.3-70B compatible)
* **Cohere Chat API** (optional)

### Rendering & Export

* iframe-based resume preview
* CSS **print media queries** for A4 export

---

## 📸 How It Works

1. User enters resume details
   *(Education, Experience, Projects, Skills, etc.)*
2. User provides their **own API key**
3. Selected resume template + AI prompt is sent to the LLM
4. LLM returns **clean HTML only**
5. Resume is rendered inside an **iframe**
6. User downloads a **print-ready PDF**

---

## 🔑 API Key Handling (Important)

This project **does NOT expose any API keys**.

* Users must enter their **own API key**
* Key is stored **locally in the browser**
* The key is **never logged, shared, or sent anywhere else**

Example:

```js
localStorage.setItem("GROQ_API_KEY", apiKeyInput.value);
```

---

## 🖨️ PDF Export (A4 Guarantee)

* Resume is rendered at **210mm × 297mm**
* CSS enforces:

  * No overflow
  * No scrolling
  * Print-safe colors
* Browser print dialog → **“Save as PDF”**

Ensures compatibility with:

* Recruiters
* ATS systems
* Email submissions

---

## 📂 Project Structure

```text
├── index.html
├── style.css
├── script.js
├── README.md
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/ai-resume-builder.git
cd ai-resume-builder
```

### 2️⃣ Open in Browser

```text
Open index.html
```

or simply **double-click `index.html`**.

### 3️⃣ Use the App

* Enter resume details
* Paste your LLM API key
* Select a template
* Click **Generate Resume**

---

## 🧪 Tested On

* **Chrome** (recommended)
* Edge
* Brave
* Firefox *(print supported, slight preview differences)*

---

## 📌 Limitations

* Frontend-only (no rate limiting)
* API usage depends on user’s own key
* Internet connection required for AI generation

---

## 🛠️ Future Improvements

* Backend proxy for stronger API security
* Job-description keyword matcher
* Resume score (ATS compatibility)
* Section drag-and-drop reordering
* Multi-language resume support

---

## 🙌 Acknowledgements

* **Groq AI**
* **Cohere**
* Open-source resume formatting standards
* ATS best-practice research

---

