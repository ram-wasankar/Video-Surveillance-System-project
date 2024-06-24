Video Surveillance System

The Video Surveillance System is a robust application designed to monitor and record video footage from multiple cameras. This system supports real-time video streaming, motion detection, and recording functionalities, making it an ideal solution for both home and business security needs.
Features

    Real-Time Video Streaming: View live video feeds from multiple cameras.
    Motion Detection: Receive alerts and start recording when motion is detected.
    Recording and Playback: Record video footage and play it back at a later time.
    Multi-Camera Support: Connect and monitor multiple cameras simultaneously.
    User Authentication: Secure access to the system with user authentication.

Getting Started

Follow these instructions to set up and run the Video Surveillance System on your local machine.
Prerequisites

    Python 3.x
    OpenCV
    Flask
    SQLite (or any other preferred database)
    Email service (for sending alerts)

Installation

    Clone the Repository

    bash

git clone https://github.com/your-username/video-surveillance-system.git
cd video-surveillance-system

Install Dependencies

Use pip to install the required dependencies.

bash

pip install -r requirements.txt

Configure the System

    Database: Set up your database (default is SQLite). Migrate the database using the provided schema.
    Email Alerts: Configure your email settings in the config.py file.
    Cameras: Add your camera URLs to the cameras.json file.

Run the Application

Start the Flask application.

bash

    python app.py

    Access the Application

    Open your web browser and go to http://localhost:5000 to access the Video Surveillance System.

Configuration

The config.py file contains configuration settings for the application, including database connections, email settings, and other options.

python

# config.py
DATABASE_URI = 'sqlite:///surveillance.db'
EMAIL_SERVER = 'smtp.example.com'
EMAIL_PORT = 587
EMAIL_USE_TLS = True
EMAIL_USERNAME = 'your-email@example.com'
EMAIL_PASSWORD = 'your-email-password'

Usage

    Dashboard: The main dashboard provides an overview of all connected cameras and their live feeds.
    Motion Detection: When motion is detected, an alert is sent via email and the recording starts automatically.
    Playback: Navigate to the recordings section to view and manage recorded footage.

Contributing

Contributions are welcome! Please follow these steps to contribute:

    Fork the repository.
    Create a new branch (git checkout -b feature/your-feature).
    Commit your changes (git commit -am 'Add new feature').
    Push to the branch (git push origin feature/your-feature).
    Open a pull request.