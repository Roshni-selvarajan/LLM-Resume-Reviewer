
# Resume Evaluator

## Project Overview

The Resume Evaluator project is designed to assist job seekers in tailoring their resumes to specific job descriptions by evaluating and providing insights on resume content. By leveraging AI capabilities, the tool identifies matching percentages, missing keywords, and offers recommendations to improve resumes in a competitive job market.

## Features

- **Job Description Input:** Users can paste a job description to evaluate their resume against.
- **PDF Resume Upload:** Supports uploading a resume in PDF format for analysis.
- **AI-Powered Evaluation:** Utilizes the Gemini Pro model to provide feedback on resume alignment with the job description.
- **Comprehensive Feedback:** Returns a matching percentage, highlights missing keywords, and provides personalized recommendations for improvement.

## Technologies Used

- **Streamlit:** For building an interactive web application.
- **Google Generative AI (Gemini Pro):** For generating content and evaluating resumes.
- **PyPDF2:** For extracting text from PDF files.
- **Python:** Core programming language for development.

## Getting Started

To run this project locally, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/resume-evaluator.git
   cd resume-evaluator
   ```

2. **Install Dependencies:**
   Make sure you have Python installed, then install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Environment Variables:**
   - Create a `.env` file in the project root.
   - Add your Google API key:
     ```
     GOOGLE_API_KEY=your_api_key_here
     ```

4. **Run the Application:**
   ```bash
   streamlit run app.py
   ```

5. **Use the Application:**
   - Open your web browser and go to `http://localhost:8501`.
   - Paste the job description and upload your resume in PDF format.
   - Click "Submit" to receive the evaluation results.

## How It Works

1. **Load Environment Variables:** The application loads API keys and other configurations from a `.env` file.
   
2. **Extract Text from PDF:** The uploaded resume is processed to extract text using PyPDF2.

3. **Generate AI Response:** The text and job description are inputted into the Gemini Pro model to generate an evaluation response.

4. **Display Results:** The application displays the matching percentage, missing keywords, final thoughts, and recommendations.

## License

This project is licensed under the MIT License, allowing for modification and distribution under specific conditions.
