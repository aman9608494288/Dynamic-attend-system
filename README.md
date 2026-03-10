# 🛡️ Dynamic Attend | Smart Attendance System

**Dynamic Attend** is a secure, real-time attendance management system designed to eliminate proxies using time-stamped, regenerating QR codes. Developed for the **BCA Program at Aryabhatta Knowledge University (AKU)**.

---

## 🚀 Key Features
* **Dynamic QR Generation:** Secure AES-encrypted QR codes refresh every 30 seconds to prevent cheating.
* **Instant Verification:** Real-time scanning and logging using the `html5-qrcode` library.
* **Automated Dashboards:** Each student receives a personalized dashboard showing real-time attendance stats (e.g., 15/30 classes).
* **Cross-Platform Sync:** Backend integration with **SQLite** ensures data is pushed directly to the database in milliseconds.

---

## 🛠️ Tech Stack
* **Frontend:** HTML5, CSS3 (Glassmorphism UI), JavaScript (ES6+).
* **Backend:** Python Flask with Flask-CORS for secure API handling.
* **Database:** SQLite for local prototyping and student data persistence.
* **Libraries:** `QRCode.js` for generation and `Html5-Qrcode` for scanning.

---

## 📂 Project Structure
```text
├── app.py              # Flask Backend API
├── home.html           # Landing Page & Intro Screen
├── login(1).html       # Multi-role Login with OTP
├── signup.html         # Student/Teacher Registration
├── dashboard.html      # Student Panel & QR Generator
├── attendance.db       # SQLite Database File
└── requirements.txt    # Python Dependencies
---
⚙️ Installation & Setup
1. Backend Setup
Clone the repository.

Install dependencies:

Bash
pip install flask flask-cors gunicorn
Run the server:

Bash
python app.py

2. Frontend Setup
Open home.html in any modern web browser.

Ensure the BASE_URL in your JavaScript files matches your local or live Flask server address.

📡 Live Deployment
Frontend: Hosted on Netlify.

Backend: Hosted on Render with a persistent SQLite disk.

👨‍💻 Developed By
IT MINDS COLLECTIVE BCA Student, CIMAGE (AKU)


---
## 👥 Role-Based Instructions

### 👨‍🏫 For Teachers
1. **Login:** Use the Teacher credentials to access the "Verificator" panel.
2. **Scanner Activation:** Click **"Activate Scanner"** to open the camera.
3. **Verification:** Scan the student's regenerating QR code.
   * *Note:* The system will automatically update the database and provide a success alert.

### 👪 For Parents
1. **Login:** Access the **"Parent Login"** via the home page.
2. **Dashboard:** Enter the student's **Roll Number** to view their live attendance percentage.
3. **Monitoring:** View the "Classes Attended vs. Total Classes" progress bar.
