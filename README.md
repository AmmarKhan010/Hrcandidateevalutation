HR Candidate Screening Assistant
A simple Streamlit web app that helps HR select candidates based on Python, data analysis, and teamwork skills by matching candidate CVs with job attributes using basic text similarity.

Features
Input required job attributes (skills, experience, education) via sidebar

Upload candidate CV as a plain text file (.txt)

Compute similarity score between job description and CV using TF-IDF and cosine similarity

Display match percentage and interview recommendation

How to Run on Google Colab
Open this notebook in Google Colab.

Replace the ngrok auth token with your own (sign up at ngrok.com if you don’t have one).

Run the provided code cell which:

Installs dependencies (streamlit, pyngrok)

Writes the Streamlit app to app.py

Sets up and authenticates ngrok

Starts a tunnel and launches the Streamlit app

Click the generated public URL to open the app.

Use the sidebar to set job requirements and upload candidate CV files.

Requirements
Python 3.x

Streamlit

pyngrok

Google Colab environment (recommended for easy ngrok tunneling)

Notes
The CV upload currently supports plain text files (.txt) only.

The matching is based on simple TF-IDF vector similarity, intended as a basic demonstration.

For advanced use, consider adding PDF/DOCX parsing and more sophisticated NLP models.

License
MIT License © Ammar Akhter Khan

