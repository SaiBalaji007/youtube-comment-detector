# YouTube Hate & Hope Comment Detector

A Flask-based web application that analyzes YouTube comments using **Machine Learning and NLP** to classify them as **Hope (Positive)** or **Hate (Negative)**.  
The system also includes an **AI assistant powered by Google Gemini** and a **YouTube video tracking dashboard** for analyzing engagement metrics.

---

## Key Features

- Secure **user authentication** (signup & login)
- **YouTube comment sentiment analysis** using ML
- **AI chatbot assistant** powered by Google Gemini
- **Video analytics tracking** (views, likes, subscribers)
- **Prediction history dashboard**
- Interactive **data visualization**

---

## Tech Stack

**Backend**
- Python
- Flask

**Machine Learning**
- scikit-learn
- transformers
- torch

**APIs**
- Google Gemini API
- YouTube Data API

**Database**
- SQLite

**Frontend**
- HTML
- CSS
- JavaScript
- Jinja2 Templates

---

## Project Structure


## Project Structure

- **app.py** – Main Flask application  
- **database.py** – Database setup and helper functions  
- **requirements.txt** – Python dependencies  
- **.env.example** – Environment variables example  

### models
- `hope_hate_model.pkl` – Pretrained sentiment model  

### services
- `gemini_chat.py` – Gemini AI chatbot logic  
- `hate_classifier.py` – Comment sentiment classifier  
- `youtube.py` – YouTube API interaction  
- `youtube_tracker.py` – Video statistics tracking  

### static
- **css/** – Stylesheets  
- **js/** – JavaScript files  
- **images/** – Images and assets  

### templates
- `base.html`
- `home.html`
- `login.html`
- `signup.html`
- `predict.html`
- `dashboard.html`
- `chatbot.html`
- `youtube_tracker.html`
- `about.html`
Installation & Setup
Clone the repository:

git clone https://github.com/BhavishyaKatariya/youtube-sentiment-ai-assistant.git # Update with your repo
cd youtube-sentiment-ai-assistant # Update with your repo name
Install Dependencies:

pip install -r requirements.txt
Set Environment Variables: Create a .env file in the root directory of your project.

GEMINI_API_KEY="your_gemini_api_key_here"
YOUTUBE_API_KEY="your_youtube_data_api_key_here"
SESSION_SECRET="a_strong_random_secret_key"
GEMINI_API_KEY: Obtain your API key from Google AI Studio.
YOUTUBE_API_KEY: Obtain your API key from the Google Cloud Console. Ensure the "YouTube Data API v3" is enabled for your project.
SESSION_SECRET: A strong, random secret key for Flask session management. You can generate one using python -c 'import os; print(os.urandom(24))'.
For deployment (e.g., on Render), set these variables directly in your hosting platform's environment settings.
Run the Application:

python app.py
The application will be available in your browser at http://0.0.0.0:5005.
---

