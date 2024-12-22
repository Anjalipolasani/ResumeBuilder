Resume Builder with Google Gemini Pro
This application tailors a user's resume to align with a given job description by leveraging the capabilities of Google’s Gemini Pro AI model. It streamlines the resume customization process, helping users quickly highlight relevant skills and experiences to increase their chances of securing interviews.



Overview
The Resume Builder project enables Purdue University Fort Wayne (PFW) Career Development Center and PFW students to simplify and enhance the resume preparation process. By integrating advanced AI-driven text generation and job readiness analysis, the system helps students present their qualifications in a way that best matches the target job description.

Key Features
Resume Upload:
Upload your current resume in .docx or .pdf format.
Job Description Analysis & Comparison:
Upload the target job description to assess how closely your current resume matches the job requirements.
A similarity score (0–100%) is provided to help gauge alignment.
Generate Enhanced Resume:
With a single click, generate a tailored resume using Google’s Gemini Pro AI model. The tool emphasizes the most relevant skills, experiences, and achievements for the selected job description.
Download Generated Resume:
Obtain the new, customized resume in .docx (and optionally .pdf) format.
How It Works
Upload Documents:
Provide your existing resume and the job description you want to target.

AI Analysis & Tailoring:
The system extracts text from the uploaded files and constructs prompts for Gemini Pro.

Gemini Pro receives the combined context and transforms the original resume into a version that highlights the most relevant qualifications.
Similarity Scoring:
The tailored resume and job description are compared to generate a similarity score. This helps you understand how well the your current skills presented in the original resume aligns with the job requirements.

Download & Refine:
Download the customized resume and, if needed, make final manual adjustments before submitting it to prospective employers.

Technology Stack
Frontend:
React
Used for building a responsive and interactive user interface.

Backend & Server:
Flask
Handles server-side logic, API endpoints, and communication between the frontend and AI services.

AI Model Integration:
Google Cloud
Integrates with Google Generative AI (Gemini Pro) for content generation and resume tailoring.

File Parsing & Processing:

PyPDF2 for extracting text from PDFs
docx2txt and python-docx for handling .docx files
Text Processing & Conversion:
TensorFlow for tokenization and text preprocessing
python-docx and headless LibreOffice for DOCX and PDF conversion

Comparison & Similarity: Custom logic to measure alignment between the candidates resume and the job description.

Setup & Deployment
Prerequisites:

Node.js installed on your machine for running the React frontend.
Python 3.x installed for running the Flask backend.
Access to the Google Generative AI API (Gemini Pro) and a valid GOOGLE_GEMINI_KEY.
1. Clone the Repository
git clone https://github.com/yourusername/resume-builder-gemini-pro.git
cd resume-builder
2. Set Environment Variables
export GOOGLE_GEMINI_KEY="your_google_gemini_api_key"
3. Frontend Setup (React)
cd Front-end/my-app
npm install    # Install frontend dependencies
npm run build  # Optionally build for production, or skip and just run locally
npm start      # Start the React development server
4. Backend Setup (Flask)
cd ../../Back-end   # Navigate back and into the backend folder
pip install -r requirements.txt   # Install backend dependencies
5. Run the Flask Server
flask run
6. Accessing the Deployed Version
A deployed version may be accessible at: http://34.132.65.232:3000/

If running locally, use:

Frontend: http://localhost:3000 Backend: http://127.0.0.1:5000

Use Cases
Career Development Centers: Help career advisors efficiently prepare students' resumes for different roles, enhancing the relevance of each application.

Students & Job Seekers:
Quickly adapt a single "master resume" to fit multiple job applications, saving time and ensuring a better match each time.
