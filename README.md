HR Candidate Screening Assistant
A streamlined Streamlit web application designed to assist HR professionals in the initial screening process. This tool evaluates candidate suitability by calculating the semantic similarity between a job description and a candidate's CV using TF-IDF and Cosine Similarity.

🚀 Features
Customizable Job Criteria: Input specific required attributes (skills, experience, education) directly via the sidebar.

CV Analysis: Support for candidate CVs in plain text (.txt) format.

Algorithmic Matching: Utilizes Scikit-learn's TfidfVectorizer to compute a match percentage.

Actionable Insights: Displays a similarity score and an automated interview recommendation based on the match.

Cloud Ready: Optimized for execution on Google Colab with integrated ngrok tunneling.

📂 Project Structure
Plaintext
hr-screening-assistant/
├── app.py              # Main Streamlit application logic
├── requirements.txt    # List of Python dependencies
├── notebooks/
│   └── colab_run.ipynb # Google Colab notebook for ngrok setup
├── data/
│   └── sample_cv.txt   # Example candidate CV for testing
└── README.md           # Project documentation and setup guide

🛠️ Requirements
To run this application, you will need:

Python 3.x

Streamlit

Scikit-learn

pyngrok (for tunneling in Colab)

💻 How to Run (Google Colab)
Open the Notebook: Load the project notebook into your Google Colab environment.

Get an Auth Token: Sign up at ngrok.com to retrieve your personal authentication token.

Execute the Code: Run the provided cells to:

Install necessary dependencies (streamlit, pyngrok).

Generate the app.py file.

Authenticate and launch the ngrok tunnel.

Access the App: Click the generated public URL (e.g., http://xxxx-xxxx.ngrok.io) to open the Streamlit interface.

📂 Usage
Define Requirements: Use the sidebar to enter key job attributes like "Python", "Data Analysis", or "Project Management".

Upload CV: Upload the candidate's CV as a .txt file.

Review Results: The app will instantly calculate the match percentage and suggest whether to proceed with an interview.

📝 Technical Notes
[!IMPORTANT]
Current Limitation: This version supports .txt files only. For production environments, it is recommended to integrate libraries like PyPDF2 or python-docx for broader file support.

The matching engine uses a basic vector-space model:

TF-IDF: Converts text into numerical vectors based on word importance.

Cosine Similarity: Measures the cosine of the angle between the Job Description vector and the CV vector.

⚖️ License
Distributed under the MIT License. © 2026 Ammar Akhter Khan
