# SIMI-Scheme_Information_Made_Intelligent-
# 🤖 SIMI AI — Scheme Information Made Intelligent

*SIMI AI* is a smart Flask webhook service that helps users discover government schemes tailored to their profile — based on caste, gender, and education. It integrates with Dialogflow to provide instant, personalized scheme recommendations, making navigating government benefits easier and more intuitive!

---

## 🌟 Features

- 🔍 Intelligent matching of user attributes (caste, gender, education) against scheme eligibility
- 📂 Loads schemes from a flexible JSON dataset (schemes_final.json)
- 🚀 Designed for smooth Dialogflow webhook integration
- 💬 Returns clear, user-friendly scheme info with benefits and application links
- 🛠️ Detailed logging for easy debugging and monitoring
- 🎯 Supports education synonyms & partial matching for better accuracy

---

## 🗂️ Project Structure

~~~ 
simi-ai/
├── app.py                  # Main Flask application with webhook logic
├── schemes_final.json      # JSON file containing schemes data
├── requirements.txt        # Project dependencies (Flask==2.3.2)
└── README.md               # This README file
~~~

## 🛠️ Getting Started

### Prerequisites

- Python 3.8 or higher
- Flask 2.3.2

### Installation

1. Clone or download the repo

bash
git clone https://github.com/yourusername/simi-ai.git
cd simi-ai

2. Install dependencies
bash
    pip install Flask==2.3.2

3. Make sure your schemes_final.json file is in the project directory.


### Running the App

Start the Flask server on port 5000:

bash
   python app.py

You should see:


csharp
  Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)


## 🧠 Behind the Scenes: Matching Logic

* Normalization: Converts inputs to lowercase and strips spaces for consistent matching
* Synonyms: Education levels match common variants like "12th", "XII", "graduate", "bachelor"
* Flexible matching: Checks both dedicated fields (like caste, gender) and free-text eligibility info
* Fallbacks: If no clear title found for a scheme, skips it to avoid irrelevant matches

![image](https://github.com/user-attachments/assets/07a71079-d6d1-462f-baf9-12fdbd502ee5)

![image](https://github.com/user-attachments/assets/181498a6-a45f-4686-87be-e4728b6ffeb7)

