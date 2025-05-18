# 🎵 Flask Song Playlist App

This is a lightweight Flask-based web application that allows users to view a list of songs from a playlist, view individual song details, and rate songs on a scale of 1 to 5.

---

## 📁 Project Structure
project-root/
│
├── data/
│ ├── playlist.json # Original song data in JSON format
│ └── playlist.csv # Normalized CSV file generated from JSON
│
├── parse_json.py # Script to normalize JSON to CSV
├── app.py # Main Flask application
├── templates/ # Jinja2 HTML templates
└── static/ # CSS, JS, assets (optional)

## 🚀 Setup Instructions

### 1. Clone the Repository

```bash
git clone <repository-url>
cd <repository-folder>

### **2. required modules**  Install Dependencies
flask
pandas
numpy
request
pytest

### **3. Convert JSON to CSV**
python parse_json.py
This will create a playlist.csv file inside the data/ directory.

**### 4. Run the Flask Application**
python app.py

> The application will start on:
http://127.0.0.1:5000


**### 5. Example Usage**
Open browser to:
http://127.0.0.1:5000

> Use the dropdown in the last column to rate a song.
> Click on View to open a detailed view of the song.
> The rating will persist during the current session.

**### 6. Application Features**
🏠 Home Page (/)
> Displays all songs with pagination

**### 7. Song Detail Page (/song/<id>)**
> View complete information about a single song
> Rate the song directly from the detail page

**### 8. Rating System**
> Users can rate songs from the home page or detail page
