# ResumeRaptor

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


---

## Tech Stack

- **Frontend & App Framework**: Streamlit (Python)
- **AI Model**: Google Gemini via `google.generativeai`
- **OCR & PDF Parsing**: `pdfplumber`, `PyPDF2`, `Poppler`, `pdf2image`
- **Web Scraping**: `Selenium`, `requests`
- **Environment Management**: `.env` (local), Streamlit Secrets (deployment)

---

## 🚀 Live Demo

Check out the live deployed app here:  
**🔗 [https://resumeraptor.streamlit.app/](https://resumeraptor.streamlit.app/)**

---

## 🧠 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Amannpy/Resume-Raptor.git
cd Resume-Raptor
