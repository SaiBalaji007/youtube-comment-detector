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

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/SaiBalaji007/youtube-hate-and-hope-comment-detector.git
cd youtube-hate-and-hope-comment-detector
2. Install dependencies
pip install -r requirements.txt
3. Configure environment variables

Create a .env file and add:

GEMINI_API_KEY=your_gemini_api_key
YOUTUBE_API_KEY=your_youtube_api_key
SESSION_SECRET=your_secret_key
4. Run the application
python app.py

The app will run at:

http://localhost:5005
Machine Learning Model

The system uses a pre-trained sentiment classification model (hope_hate_model.pkl) to analyze YouTube comments and classify them into:

Hope → Positive sentiment

Hate → Negative sentiment

Security

Password hashing using Werkzeug

Secure session-based authentication

Protected routes for logged-in users

API keys managed through environment variables

License

This project is built for educational and learning purposes.
