# 🎙️ TalkMetrics

**TalkMetrics** is a full-stack web application designed to analyze YouTube video comments and perform sentiment analysis using machine learning.

## 🚀 Features

- 🎥 Fetches comments from YouTube videos using the YouTube Data API.
- 🧠 Analyzes sentiment of each comment (Positive, Neutral, Negative) using a deep learning model.
- 📊 Displays sentiment distribution and comment data on a user-friendly dashboard.
- 🔁 Full-stack integration with Flask (Backend) and React (Frontend).

## 📦 Technologies Used

### Backend

- Python
- Flask
- TensorFlow / Keras
- Google API Client
- Flask-CORS
- dotenv

### Frontend

- React
- Bootstrap
- Axios

## 📁 Project Structure

```
TalkMetrics/
├── Backend/
│   ├── app.py
│   ├── sentiment_prediction_model.keras
│   ├── sentiment_tokenizer.pickle
│   ├── requirements.txt
│   └── .env
├── Fronted/
│   ├── public/
│   ├── src/
│   │   ├── App.js
│   │   ├── components/
│   │   └── index.js
│   └── package.json
└── README.md
```

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/Gamanaram-Choudhary/TalkMetrics.git
cd TalkMetrics
```

### 2. Backend Setup

```bash
cd Backend
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install -r requirements.txt
```

Create a `.env` file with your YouTube API key:

```
YOUTUBE_API=YOUR_API_KEY_HERE
```

Run the Flask server:

```bash
python app.py
```

### 3. Frontend Setup

```bash
cd ../Fronted
npm install
npm start
```

## 📡 API Endpoints

### `POST /get_comments`

Fetches comments from a YouTube video.

### `POST /sentiment`

Analyzes sentiment of provided comments.

## 📜 License

MIT License

---

> Made with ❤️ by Gamanaram Choudhary
