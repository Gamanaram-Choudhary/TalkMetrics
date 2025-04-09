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

Copyright (c) [2025] [Gamanaram Choudhary]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

> Made with ❤️ by Gamanaram Choudhary
