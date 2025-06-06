# 🧠 Resume Standardizer: AI-Powered CV Formatter

Transform unstructured resumes into clean, company-standardized formats using the power of GenAI and intelligent document parsing.

🔗 **Try the App Live**: [Resume Builder app](https://resume-builder-aml-project.streamlit.app/)

---

## 🚀 About the Project

Companies often receive resumes in various formats—PDFs, DOCXs, and images—each with different structures and styles. After hiring, organizations frequently need to convert these diverse resumes into a **uniform company-specific CV format** for internal documentation, onboarding, and record-keeping.

**Resume Standardizer** is designed specifically to solve this problem. It enables companies to:

- Upload resumes in any format (PDF, DOCX, or image),
- Automatically extract key candidate details such as education, experience, and skills,
- Generate a clean, structured CV tailored to the company’s preferred template.

This project was developed as part of the **Applied Machine Learning course** (by **Prof. Raghav Kulkarni**), with a focus on solving real-world HR documentation challenges using GenAI.

---

## 🛠️ Features

- ✅ Uploads PDF, DOCX, or image-based resumes
- 🎯 Converts resumes into selectable company templates
- 🔐 Trial mode available or use your Gemini API key
- ⚡ Fast response time via Gemini 2.0 Flash
- 📝 Extracts and formats data using custom NLP pipelines

---

## 🧬 How It Works

1. **Input**: Resume file uploaded (PDF, DOCX, or image).
2. **Parsing**: Raw text extracted via PDF/image parsers and preprocessed.
3. **Field Extraction**: NLP and regex-based extractors identify structured details.
4. **LLM Enrichment**: Gemini 2.0 Flash helps parse ambiguous or complex fields.
5. **Formatting**: Data is injected into a company-specific CV layout.
6. **Output**: Ready-to-download standardized resume.

---

## 🔧 Tech Stack

- **Frontend**: Streamlit
- **LLM**: Gemini 2.0 Flash (low-latency, supports multimodal input)
- **Resume Parsing**: 
  - `pdfplumber`, `PyMuPDF` for PDFs
  - `docx` for Word files
  - `cv2`, `PIL` for image-based resumes
- **Template Generation**: `reportlab`, `BytesIO`, `zipfile`
- **Custom Code**: For field extraction, docx2pdf conversion, section segmentation, and formatting

---

## 🎯 Why Gemini?

We chose **Gemini 2.0 Flash** because:
- It handles images and text inputs effectively.
- It offers low latency ideal for near-real-time applications.
- Despite its token limitations, it was sufficient for our resume parsing task.

---

## 🔍 Challenges We Tackled

- 🧩 Dealing with various document structures and layouts
- 🕵️ Identifying logical sections like Education vs Experience from inconsistent labels
- 📸 Handling embedded content (e.g., profile pictures, logos)
- 🧠 Differentiating between job responsibilities vs. project details

---

## 📈 Future Scope

- 🌍 **Multilingual support** using mBERT / XLM-R
- 🧩 **API integration** for HR systems (ATS, Workday, etc.)
- 🧠 **Resume scoring** based on job descriptions using semantic matching
- 📊 Improved **scalability** with parallelized document handling

---

## 👨‍💻 Team & Contributions

| Name               | Role                                                                 |
|--------------------|----------------------------------------------------------------------|
| **Aniket Tiwari**  | UI design, Streamlit integration, full app deployment                |
| **Deepanshu Mittal** | Resume parsing logic, PDF & DOCX handling, text extraction         |
| **Kironmoy Roy**   | Template filler logic, structured format generation, formatting logic|

---

## 💬 Quote We Believe In

> _"Alone we can do so little; together we can do so much."_  
> — Helen Keller

---

## 📂 License

This project is academic in nature and currently not under a formal open-source license. For collaboration or reuse, please contact the authors.