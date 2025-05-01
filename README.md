# Resume Raptor

**ResumeRaptor** is an AI-powered resume analysis and feedback tool that leverages **Google Gemini AI**, **OCR**, and **web scraping** to help candidates optimize their resumes based on job roles and descriptions. It supports PDF and DOCX files, making it accessible and flexible for modern job seekers.

---

## Features

- **Resume Analysis with Google Gemini AI**  
  Get instant AI-generated insights and suggestions to improve your resume.

- **Job Description Matching**  
  Match resumes against specific job roles or descriptions for relevance scoring.

- **Multi-format Parsing**  
  Extracts text from PDFs and DOCX files, including image-based resumes using OCR.

- **LinkedIn Scraper (Beta)**  
  Fetch role-specific responsibilities and skills directly from LinkedIn job posts.

- **Real-time Feedback**  
  Intuitive UI built with Streamlit provides quick and interactive analysis.

---

## Screenshots

![resume1](https://github.com/user-attachments/assets/522fa145-de5c-4531-9ffe-c94085bf883d)  
![resume2](https://github.com/user-attachments/assets/91f481c0-8dd1-4554-bbff-ddcade8f9676)  
![resume3](https://github.com/user-attachments/assets/21cb7cc0-2b31-4bae-84e7-a89b3858fa57)

---

## Tech Stack

- **App Framework**: Streamlit (Python)
- **AI Model**: Google Gemini via `google.generativeai`
- **OCR & Parsing**: `pdfplumber`, `PyPDF2`, `Poppler`, `pdf2image`
- **Web Scraping**: `Selenium`, `requests`
- **Secrets Management**: `.env` (local) & Streamlit Secrets (for deployment)

---

## 🚀 Live Demo

Explore the app here:  
**🔗 [https://resumeraptor.streamlit.app/](https://resumeraptor.streamlit.app/)**

> Note: Due to recent behavior on Streamlit Cloud around environment variable resolution, some AI analysis functionality may not be active in the hosted version. For full capability, it's recommended to run the app locally.

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Amannpy/Resume-Raptor.git
cd Resume-Raptor
2. Install Dependencies
It’s recommended to use a virtual environment.

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
3. Add API Keys
Create a .env file inside the utils/ directory with the following contents:

env
Copy
Edit
GOOGLE_API_KEY=your_google_gemini_api_key
OPENROUTER_API_KEY=your_openrouter_api_key
The .env file is used to securely load environment variables. It is excluded from version control via .gitignore.

Make sure your code uses load_dotenv(dotenv_path='utils/.env') to load it correctly.

Deployment on Streamlit Cloud
If deploying to Streamlit Cloud, manually add your secrets in the Streamlit Secrets Manager.

Use the following TOML format:

toml
Copy
Edit
[secrets]
GOOGLE_API_KEY = "your_google_gemini_api_key"
OPENROUTER_API_KEY = "your_openrouter_api_key"
These are automatically injected as environment variables at runtime. You do not need a .env file during deployment.


