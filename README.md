# 🩺 VitalSync – AI-Enabled Virtual Health Assistant for Refugees

🏆 **Top 5 Finalist – PhaseShift Hackathon, BMS College of Engineering (120 teams)**

Refugees and displaced communities often lack access to reliable healthcare.  
**VitalSync** is an AI-powered healthcare assistant designed to provide accessible medical guidance through AI symptom analysis, voice interaction, and medical report processing.

---

## ✨ Key Features

- **Medical Report Simplification**  
  Upload PDF medical reports, automatically extract text, and generate a secure SHA-256 hash to ensure data integrity.

- **AI Symptom Checker with Triage**  
  Input symptoms via text or voice to receive AI-powered guidance with severity indicators:  
  🔴 Emergency | 🟡 Moderate | 🟢 Mild.

- **Voice Input & Output**  
  Speech-to-Text and Text-to-Speech support improves accessibility for users with low literacy and multilingual needs.

- **Camera-Based Anemia Detection**  
  Prototype system using OpenCV to analyze eye/lip images for potential anemia indicators.

- **Vaccination Tracking**  
  Store and manage personalized vaccination records linked to a user ID using SQLite.

- **Nearby Humanitarian Health Services**  
  Finds nearby clinics and healthcare services using a dataset (`clinics.json`).

- **Downloadable Health Records**  
  Generate a personal PDF containing chats, uploaded medical reports, and verification hashes.

---

## 🛠️ Tech Stack

**Frontend / UI**
- Streamlit

**AI / ML**
- Google Gemini API (`google-generativeai`)

**Backend & Database**
- SQLite3

**Document Processing**
- pdfplumber
- fpdf

**Voice Processing**
- Vosk (Speech-to-Text)
- gTTS (Text-to-Speech)

**Computer Vision**
- OpenCV (`cv2`)

**Environment Management**
- python-dotenv

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/vitalsync-ai-health-assistant.git
cd vitalsync-ai-health-assistant
````

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it:

**Mac / Linux**

```bash
source venv/bin/activate
```

**Windows**

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add your Gemini API key

Create a `.env` file:

```
GOOGLE_API_KEY=your_api_key_here
```

---

## 🚀 Usage

Run the Streamlit app:

```bash
streamlit run app.py
```

Open in your browser:

```
http://localhost:8501
```

---

## 📁 Project Structure

```
app.py                # Main Streamlit application
clinics.json          # Dataset of nearby health services
database.db           # SQLite database
symptom_checker.py    # AI triage logic
anemia_detector.py    # OpenCV anemia detection prototype
requirements.txt      # Project dependencies
```

---

## 👨‍💻 Authors

Built with ❤️ during **PhaseShift Hackathon**.

Team **VitalSync**
