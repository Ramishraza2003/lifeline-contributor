<div align="center">

# 🩺 LifeLine+

### AI-Powered Mobile Healthcare Platform for Pakistan

*Digitizing prescriptions. Simplifying healthcare. Saving lives.*

[![Flutter](https://img.shields.io/badge/Frontend-Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
[![Flask](https://img.shields.io/badge/Backend-Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Firebase](https://img.shields.io/badge/Database-Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Python](https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](#license)

[Overview](#-overview) • [Features](#-key-features) • [Tech Stack](#-tech-stack) • [Architecture](#-architecture) • [Getting Started](#-getting-started) • [Team](#-team)

</div>

---

## 📖 Overview

**LifeLine+** is a Final Year Project (2022–2026, The University of Faisalabad) that reimagines how patients in Pakistan interact with the healthcare system. By combining **OCR**, **NLP**, and a **Flutter + Flask** architecture, LifeLine+ turns a photo of a handwritten prescription into a structured, searchable digital health record — bridging the gap between traditional paper-based prescriptions and modern digital healthcare.

The platform is built for the realities of the local healthcare context: overworked clinics, handwritten prescriptions, fragmented medical history, and limited pharmacy connectivity.

<div align="center">
<i>📱 Screenshot placeholder — add app screenshots/GIFs here once available</i>
</div>

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🔍 **Prescription Digitization** | OCR + NLP pipeline extracts medicines, dosage, and instructions from scanned/photographed prescriptions |
| 🗂️ **Digital Health Records** | Centralized, chronological medical history accessible anytime, anywhere |
| 💊 **Pharmacy Integration** | Connects digitized prescriptions directly with partner pharmacies |
| ⏰ **Medicine Reminders** | Smart, scheduled notifications so patients never miss a dose |
| 🚨 **Emergency Support** | Quick access to critical health information during emergencies |
| 🔐 **Secure Cloud Sync** | Firebase-backed authentication and real-time data storage |

---

## 🧱 Tech Stack

<div align="center">

| Layer | Technology |
|---|---|
| **Frontend** | Flutter (Dart) |
| **Backend** | Python, Flask (REST API) |
| **Database / Auth** | Firebase |
| **OCR Engine** | Tesseract / custom OCR pipeline |
| **NLP** | Text extraction & entity recognition for medicine/dosage parsing |
| **Version Control** | Git & GitHub |

</div>

---

## 🏗️ Architecture

```
┌─────────────────┐        REST API        ┌──────────────────┐
│  Flutter App     │◄──────────────────────►│  Flask Backend    │
│  (Mobile Client) │                        │  (API + Business  │
│                  │                        │   Logic)          │
└────────┬─────────┘                        └────────┬─────────┘
         │                                            │
         │  Auth / Realtime Sync                      │  OCR + NLP
         ▼                                            ▼
┌─────────────────┐                         ┌──────────────────┐
│    Firebase      │                        │  OCR/NLP Engine   │
│ (Auth, Firestore,│                        │  (Prescription     │
│   Storage)       │                        │   Processing)      │
└─────────────────┘                         └──────────────────┘
```

**Core Modules:**
- **System Core & AI** — prescription parsing pipeline and intelligence layer
- **Backend & API Infrastructure** — Flask REST services, data flow, and integrations
- **Extended Modules** — pharmacy integration, reminders, and emergency support features

---

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (latest stable)
- Python 3.9+
- Firebase project credentials
- Android Studio / VS Code

### Backend Setup
```bash
git clone https://github.com/Ramishraza2003/lifeline-contributor.git
cd lifeline-contributor/backend

# Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the Flask server
python app.py
```

### Frontend Setup
```bash
cd lifeline-contributor/frontend

# Install Flutter dependencies
flutter pub get

# Run the app
flutter run
```

### Firebase Configuration
1. Create a project on the [Firebase Console](https://console.firebase.google.com/)
2. Add `google-services.json` (Android) / `GoogleService-Info.plist` (iOS) to the appropriate directories
3. Enable Authentication and Firestore/Realtime Database

---

## 📁 Project Structure

```
lifeline-contributor/
├── backend/
│   ├── app.py
│   ├── routes/
│   ├── models/
│   └── ocr_nlp/
├── frontend/
│   ├── lib/
│   ├── assets/
│   └── pubspec.yaml
└── docs/
```

---

## 🗺️ Roadmap

- [x] Core OCR/NLP prescription pipeline
- [x] Digital health records module
- [x] Medicine reminder system
- [ ] Pharmacy partner API integrations
- [ ] Multi-language OCR support (Urdu prescriptions)
- [ ] Telemedicine module

---

## 👥 Team

This project was developed as a Final Year Project at **The University of Faisalabad** (Batch 2022–2026), under the supervision of **Sabahat Tasneem**.

| Name | Role |
|---|---|
| **Ramish Raza** | Backend & API Infrastructure |
| **Najam Ul Hassan** | System Core & AI |
| **Abdurrehman Ilyas** | Extended Modules |

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the [issues page](../../issues).

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

**LifeLine+** — built with ❤️ for a healthier, more connected Pakistan.

</div>
