# Resume-Application-Tracking-System(ATS)

### An IIntelligent Applicant Tracking System (ATS) using Google's Generative AI. It analyzes resumes against job descriptions, providing valuable feedback to job seekers.

# Outputs
![Screenshot (230)](https://github.com/Shreya-Reddy-A/Resume-Application-Tracking-System-ATS/assets/122392746/65f6e846-20e3-4a35-819c-3fbd8945c332)
![Screenshot (231)](https://github.com/Shreya-Reddy-A/Resume-Application-Tracking-System-ATS/assets/122392746/dade0467-ab31-46cd-a7f3-8e8e6e9c6e92)
![Screenshot (232)](https://github.com/Shreya-Reddy-A/Resume-Application-Tracking-System-ATS/assets/122392746/919c8a0e-648b-44ed-887a-51d9a337a088)


# Features
- User authentication
- PDF resume parsing
- Job description using Google's Gemini-Pro AI model
- Percentage match visualization
- Missing keywords identification
- Profile summary generation
- Chat history storage and retrieval
- Responsive Streamlit web interface

# Getting Started
To get started follow these steps:
1. **Clone the Repository**:
   - Clone this repository to your local machine.
     ```
     git clone https://github.com/Shreya-Reddy-A/Resume-Application-Tracking-System-ATS.git
     ```

2. **Install Dependencies**:
   - Navigate into the cloned directory and install the necessary dependencies.
     ```
     cd Resume-Application-Tracking-System-ATS
     pip install -r requirements.txt
     ```
3. **Set Up Environment Variables**
   - Rename `.env.local` file in the project root directory to `.env`.
   - Add your Google API key to the `.env` file:
     ```
     GOOGLE_API_KEY=your_google_api_key_here
     ```
4. **Prepare Your Resume**:
 - Ensure you have your resume saved as a PDF file.
  
5. **Run the Application**
   - Start the Streamlit app by running:
     ```
     streamlit run app.py
     ```
6. **Login Credentials**
   - Use these credentials to access the application.
     ```
     username: admin
     password: admin123
     ```
     #### Disclaimer: The application will show an error after clicking the submit button due to API key. Kindly generate one and add it to see the results. 
     
# Usage

1. Log in using the provided credentials or create a new account.
2. Enter the company name and job role.
3. Paste the job description in the text area.
4. Upload your resume in PDF format.
5. Click "Submit" to get an analysis of your resume.

# Features Explained

### Authentication
- The app uses `streamlit-authenticator` for user authentication.
- Predefined usernames and passwords are stored in the script.

### Resume Parsing
- PyPDF2 is used to extract text from uploaded PDF resumes.

### AI-Powered Analysis
Google's Generative AI (Gemini-Pro model) analyzes the resume against the job description, providing:
- JD Match percentage
- Missing keywords
- Profile summary

### Visual Feedback
- A circular progress indicator visually represents the JD Match percentage.

### Chat History
- Previous analyses are stored and can be accessed from the sidebar.

# Dependencies
- streamlit
- PyPDF2
- google.generativeai
- python-dotenv
- streamlit-authenticator
