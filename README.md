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
