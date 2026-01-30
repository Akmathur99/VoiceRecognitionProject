# Voice Recognition Sign-In System 🎙️

A Python-based **voice recognition prototype** that authenticates users by converting spoken audio into text and validating it against keywords stored in a database.

---

## Features

- Convert audio files into text using **Google Speech Recognition API**  
- Compare spoken keywords against stored user data in a **SQLite database**  
- Retry logic for failed recognition attempts  
- Assign random valid English keywords to users without pre-set words  
- Keep track of signed-in users  

---

## Tech Stack

- **Python 3**  
- `speech_recognition` library  
- `cs50` SQL wrapper for SQLite  
- `sounddevice` & `wavio` for audio handling  
- Google Speech API  

---

## How It Works

1. User provides an **audio file** as input  
2. The system converts the audio to text using Google Speech Recognition  
3. The spoken word is **compared to stored keywords** in the database  
4. If it matches, the user is marked as **signed in**  
5. If no keyword exists for a user, the system generates a **random valid English word** and updates the database  

---

## Setup Instructions

1. Clone the repo:
```bash
git clone <your-repo-url>
cd <repo-folder>
