# Resume Building Workshop by **KRIYA-TECHNOVA**

> ### Brought to you by the **KRIYA-TECHNOVA** club (AIML Department)

Welcome to the Resume Building Workshop resource repository! 

This repository contains all the templates, guides, and checklists you need to build a professional, ATS-friendly resume for software engineering, internship, and related roles.

## What's Inside?

- **LaTeX Template:** A clean, ATS-friendly LaTeX template ready to use in Overleaf.
- **DOCX Template:** A Microsoft Word template (check the `templates/` folder).
- **Resume Guide:** Comprehensive best practices for writing your resume.
- **Resume Checklist:** A checklist to review your resume before hitting submit.



## Quick Start

### Option 1 — LaTeX / Overleaf

1. Open [Overleaf](https://www.overleaf.com/).
2. Create a **New Project** -> **Blank Project**.
3. Open the `latex/resume-template.tex` file in this repository, copy its contents, and paste it into your Overleaf `main.tex` file.
4. Replace the sample information with your own details (look for the comments!).
5. Click **Recompile**.
6. Download the generated PDF.
7. **Read the PDF carefully before submitting anywhere!**

### Option 2 — DOCX

1. Navigate to the `templates/` folder in this repository.
2. Download the provided DOCX template.
3. Open the DOCX template in Microsoft Word or Google Docs and replace the sample content.
4. Export or Save As a PDF.
5. **Read the PDF carefully before submitting anywhere!**

### Option 3 — FlowCV

1. Go to [FlowCV.com](https://flowcv.com/).
2. Create a free account.
3. Start a new resume and fill in your details section by section.
4. Choose a clean, single-column, professional template (avoid multi-column or heavily colorful ones).
5. Customize the formatting to match the guidelines in our [Resume Guide](docs/resume-guide.md).
6. Export the final resume as a PDF.
7. **Read the PDF carefully before submitting anywhere!**

## Resume Best Practices

For a full breakdown of what to include (and what to leave out), please read our detailed [Resume Guide](docs/resume-guide.md).

Before you submit your resume, make sure you go through the [Resume Checklist](docs/resume-checklist.md).

## How to Create a Shareable Resume Link

If a recruiter or application portal asks for a link to your resume instead of a PDF upload, you can easily create one using Google Drive:

1. Open **Google Drive**.
2. Upload your final exported `.pdf` resume.
3. Right-click the uploaded PDF file and select **Share**.
4. Under "General access", change the setting from "Restricted" to **"Anyone with the link"**.
5. Make sure the permission role is set to **Viewer** (do not give Editor access).
6. Click **Copy link** and share it!

## Bonus: Check Your ATS Score Locally

During the workshop, we demonstrated how to test your resume against a job description using an open-source ATS scanner.

**What is an ATS?**
ATS stands for Applicant Tracking System. It is software used by companies to automatically screen and filter resumes before a recruiter reviews them.

**What is an ATS score?**
An ATS score is a measure of how well your resume matches a particular job description according to factors such as keywords, skills, experience, education, and formatting.

### Setup Instructions

1. **Verify Prerequisites:** Make sure you have Python (pip) and Git installed.
   ```bash
   pip --version
   git --version
   ```

2. **Clone the Open ATS Repository:**
   ```bash
   git clone https://github.com/jlynshue/open-ats.git
   ```

3. **Install Open ATS:**
   ```bash
   python -m pip install -e .
   ```

4. **Run the ATS Scan:**
   Prepare your exported `resume.pdf` and a `job.txt` file containing the job description you are targeting. Then run:
   ```bash
   open-ats scan --resume "E:\ATS\resume.pdf" --job-description "E:\ATS\job.txt" --output "E:\ATS\report.json"
   ```
   *(Replace the `E:\ATS\...` paths above with the actual locations of your files).*
