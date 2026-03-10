🛡️ Dynamic Attend | Smart Attendance System
Dynamic Attend is a secure, real-time attendance management system designed to eliminate proxies using time-stamped, regenerating QR codes. This project was specifically developed for the BCA Program at Aryabhatta Knowledge University (AKU).

🚀 Key Features
Dynamic QR Generation: Secure AES-encrypted QR codes refresh every 30 seconds to prevent cheating and proxies.

Instant Verification: Real-time scanning and logging using the html5-qrcode library for millisecond-fast processing.

Automated Dashboards: Students receive a personalized dashboard showing live attendance stats (e.g., 15/30 classes).

Cross-Platform Sync: Backend integration with SQLite ensures all data is synchronized across devices instantly.

🛠️ Tech Stack
Frontend: HTML5, CSS3 (Glassmorphism UI), and JavaScript (ES6+).

Backend: Python Flask with Flask-CORS for secure API communication.

Database: SQLite for efficient student data persistence and rapid prototyping.

Libraries: QRCode.js for generation and Html5-Qrcode for camera-based scanning.

📂 Project Structure
Plaintext
├── app.py              # Flask Backend API (Python)
├── home.html           # Landing Page with futuristic intro screen
├── login(1).html       # Unified Login portal with OTP authentication
├── signup.html         # User Registration (Student, Teacher, Parent)
├── dashboard.html      # Dynamic Student Panel & QR Generator/Scanner
├── attendance.db       # SQLite database storing student records
└── requirements.txt    # Python library dependencies list

⚙️ Installation & Setup
1. Backend Setup
Clone the Repository: Download the project files to your local directory.

Install Dependencies: Run the following command in your terminal:

Bash
pip install flask flask-cors gunicorn
Run the Server: Start the API by executing:

Bash
python app.py
2. Frontend Setup
Launch: Open home.html in any modern web browser.

Configuration: Update the BASE_URL in your JavaScript files to match your server address (local http://127.0.0.1:5000 or live Render URL).

📡 Live Deployment
Frontend: Hosted on Netlify for high-speed static delivery.

Backend: Hosted on Render utilizing a persistent SQLite disk for data integrity.

👥 Role-Based Instructions
👨‍🏫 For Teachers
Login: Access the "Verificator" panel using your authorized credentials.

Scanner Activation: Click the "Activate Scanner" button to initiate the camera feed.

Verification: Scan a student's live QR code; the system updates the database automatically and provides a success alert.

👪 For Parents
Login: Use the "Parent Login" option on the home page.

Dashboard: Enter the student's Roll Number to fetch live attendance data.

Monitoring: Track attendance progress via the "Classes Attended vs. Total Classes" visual progress bar.

👨‍💻 Developed By
Team: IT MINDS COLLECTIVE

Lead: BCA Student, CIMAGE

Affiliation: Aryabhatta Knowledge University (AKU)
