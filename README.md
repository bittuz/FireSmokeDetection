# Fire & Smoke Detection 🔥💨

A Flask-based web application that detects **fire and smoke** from images and video streams using a YOLO (You Only Look Once) model.

---

## 🚀 Features
- Detects **fire and smoke** in real-time.
- Built with **Flask** for easy deployment.
- Uses **YOLO object detection** for accurate results.
- Lightweight and easy to set up.

---

## 📂 Project Structure
FireSmokeDetection/
│── static/ # CSS, JS, and images
│── templates/ # HTML templates
│── models/ # YOLO model weights
│── app.py (not uploaded) # Flask main file (you create this locally)
│── yolo_detect.py (local)# Detection logic (not uploaded due to secrets)
│── requirements.txt # Python dependencies
│── README.md # Project documentation


---

## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/bittuz/FireSmokeDetection.git
   cd FireSmokeDetection
2.Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows

Install dependencies
pip install -r requirements.txt

▶️ Running the Project

Since app.py and yolo_detect.py are not uploaded (for security reasons), you need to create them locally.

Create app.py (Flask entry point):

from flask import Flask, render_template
app = Flask(__name__)

@app.route('/')
def index():
    return render_template("index.html")

if __name__ == "__main__":
    app.run(debug=True)

Run Flask server

python app.py

Open browser at:

http://127.0.0.1:5000

📖 Notes

The detection logic (yolo_detect.py) and Twilio integration are excluded to prevent secret exposure.

Replace them locally with your own detection pipeline.

For deployment, store secrets in environment variables (.env file) instead of hardcoding.

📜 License

This project is open-source and available under the MIT License.


---

👉 Do you want me to also **rewrite `app.py` and `yolo_detect.py` templates** (safe, without your Twilio secret) so you can still share them in GitHub?
