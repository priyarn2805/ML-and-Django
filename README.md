# This is django project where we built full-stack application which will classify radiation with svm model and we can download the csv file (Data used for prediction)

# 🌌 Gamma-Hadron Particle Classifier

A Machine Learning web application built with *Django* to classify high-energy particles (Gamma vs. Hadron) using data from the MAGIC Gamma Telescope.

## 🚀 Key Features

* *Real-time Classification:* Integrated ML model for instant prediction.
* *Django Integration:* Logic handled within views.py for seamless request processing.
* *Data Persistence:* Automatic logging of inputs and results to the database.

## 🛠️ Tech Stack

* *Backend:* Django (Python)
* *Machine Learning:* Scikit-Learn (SVM)
* *Database:* SQLite
* *Data Source:* MAGIC Gamma Telescope Dataset 

## 🏗️ Implementation Details

### Model Integration (views.py)

The application loads a serialized model (.pkl or .joblib) and processes form data:

python
def predict_view(request):
    # 1. Capture telescope parameters from form
    # 2. model.predict() determines if it is 'Gamma' or 'Hadron'
    # 3. Results are saved to the database via Django Models
    # 4. Result is rendered to the UI



### Database Connection

All prediction history is stored in the database, tracking:

* *Input Features:* fLength, fWidth, fSize, etc.
* *Classification:* Gamma (Signal) or Hadron (Background).
* *Timestamp:* For historical data tracking.

## 📋 Quick Setup

1. *Install:* pip install -r requirements.txt
2. *Migrate DB:* python manage.py migrate
3. *Run:* python manage.py runserver
---

![WhatsApp Image 2026-02-05 at 9 42 24 PM](https://github.com/user-attachments/assets/c5568ab3-3941-4e24-9050-b861a9c6498e)
![WhatsApp Image 2026-02-05 at 9 42 24](https://github.com/user-attachments/assets/4bb72a17-5e5d-42a3-b5a5-884b11034c4a)
![WhatsApp Image 2026-02-05 at 3 36 02 PM](https://github.com/user-attachments/assets/c12a6ec0-b867-4699-ba59-23d570a7642c)
![WhatsApp Image 2026-02-05 at 3 36 03 PM](https://github.com/user-attachments/assets/6c3a5695-5577-49a3-9720-281319bb0dc9)
![WhatsApp Image 2026-02-05 at 3 40 36 PM](https://github.com/user-attachments/assets/5f5a8bba-1cc9-4fe5-8a4a-71d5934dd822)
