**AI Powered Smart Fitness Assistant and Calorie Recommendation System**
**Team 16**
# FitSmart AI

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/flask-2.0+-blue.svg)](https://flask.palletsprojects.com/)

FitSmart AI is a web-based fitness application that uses artificial intelligence to provide personalized health, nutrition, and workout insights. The system combines traditional fitness metrics with computer vision and AI-driven analysis to help users track progress and improve overall wellness.

## Features

###  Core Functionality

* User authentication with secure login and registration
* Fitness assessment with BMI calculation and fitness scoring
* Nutrition analysis using AI-based food image recognition
* Workout form and repetition analysis using pose estimation
* Progress tracking with visual charts and historical data

###  AI-Powered Insights

* Personalized fitness and diet recommendations
* Real-time posture and workout feedback
* Intelligent analysis of food images for nutritional estimation

### User Experience

* Responsive, mobile-friendly interface
* Clean and intuitive dashboard
* Real-time notifications for user actions

## 🛠️ Technology Stack

### Backend

* **Framework**: Flask
* **Database**: SQLite
* **Authentication**: Session-based authentication
* **API Integration**: OpenAI Vision API

### AI / ML

* **Pose Estimation**: MediaPipe
* **Image Processing**: OpenCV, PIL
* **ML Models**: Pre-trained posture and workout analysis models (.pkl)

### Frontend

* **Templates**: Jinja2
* **Styling**: Bootstrap 5
* **Icons**: Bootstrap Icons

## Prerequisites

* Python 3.8 or higher
* pip
* OpenAI API key (for nutrition analysis)
* Webcam (optional, for workout analysis)

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/BEProjects_2026.git
cd BEProjects_2026/Team_16
```

### 2. Create and Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

If `requirements.txt` is not available:

```bash
pip install flask opencv-python mediapipe openai pillow
```

### 4. Environment Setup

Create a `.env` file:

```env
OPENAI_API_KEY=your_api_key_here
SECRET_KEY=your_secret_key_here
FLASK_ENV=development
```

### 5. Run the Application

```bash
python app.py
```

Open `http://localhost:5000` in your browser.

## Usage

1. Register or log in to the system
2. Complete fitness assessment
3. Upload food images for nutrition analysis
4. Upload workout videos for posture and repetition analysis
5. Track progress through dashboards and charts

## Project Structure

```
Team_16/
├── app.py
├── README.md
├── models/
│   ├── posture.pkl
│   └── workout.pkl
├── static/
│   ├── css/
│   ├── js/
│   └── images/
├── templates/
│   ├── base.html
│   ├── dashboard.html
│   ├── assessment.html
│   ├── nutrition.html
│   ├── workouts.html
│   ├── progress.html
│   ├── login.html
│   └── signup.html
└── uploads_workouts/
```

##  Configuration

* `OPENAI_API_KEY`: Required for nutrition analysis
* `SECRET_KEY`: Flask session security key
* `FLASK_ENV`: Development or production mode

## License

This project is licensed under the MIT License.

## Acknowledgments

* OpenAI for Vision API
* Google MediaPipe
* Flask and Bootstrap communities
