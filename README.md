# ViQu
## Raspberry Pi 3-based Interview/Viva Bot Using Natural Language Processing

ViQu is an innovative interview/viva bot designed to automate technical interviews and vivas using Natural Language Processing (NLP). Built on a Raspberry Pi 3, ViQu leverages the Google Speech Engine and the lightweight eSpeak engine to provide accurate speech recognition and text-to-speech functionalities. The system not only asks questions but also marks candidates' answers using NLP techniques like keyword matching and fuzzy string matching.

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Technologies](#technologies)
- [Installation & Setup](#installation--setup)
- [Future Work](#future-work)
- [License](#license)

---

## Overview

In today's world, automation can streamline tasks that are often repetitive and time-consuming. ViQu was developed to remove the intimidation factor of face-to-face interviews and vivas by automating the process. The bot conducts interviews by:
- Randomly generating quizzes from a pre-built question bank (covering fill-in-the-blanks, true/false, multiple choice, and one-word answers).
- Evaluating responses using NLP techniques (including fuzzy matching with the fuzzywuzzy library).
- Generating a digitized marksheet with student roll numbers and scores.

This project was developed as a part of a senior undergraduate initiative, aiming to make technical interviews more efficient and less biased while also laying the foundation for further exploration in data analytics and machine learning.

---

## Key Features

- **Automated Interview Process:** Conducts interviews/vivas without human intervention.
- **Speech Recognition & Synthesis:** Utilizes both Google Speech Engine and eSpeak for converting speech-to-text and vice versa.
- **NLP-Powered Marking:** Uses keyword and fuzzy matching to assess candidate responses accurately.
- **Diverse Question Bank:** Supports various question types (fill-in-the-blanks, true/false, multiple choice, one-word answers) categorized by difficulty level.
- **Digitized Result Sheets:** Automatically generates spreadsheets with marks against student roll numbers.

---

## Technologies

- **Hardware:**
  - Raspberry Pi 3: A mini computer that serves as the platform for running the software and integrating sensors.
- **Software & Libraries:**
  - **Programming Language:** Python
  - **Speech Engines:** Google Speech Engine and eSpeak
  - **NLP Libraries:** Includes libraries for keyword matching and fuzzy matching (e.g., fuzzywuzzy)
  - **Python Libraries:** `speech_recognition`, `talkey`, and others to facilitate speech processing and text analysis

---

## Installation & Setup

### Prerequisites
- Raspberry Pi 3 set up with Raspbian (or your preferred Linux distro)
- Python 3.x installed
- Internet connection (for installing dependencies and using online speech engines)

### Installation Steps

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/shreya1297/ViQu.git
   cd ViQu

2. Install Required Python Libraries: Ensure you have pip installed, then run:

pip install -r requirements.txt

### 3. **Run the Bot**:
   To start the bot, execute the following command in your terminal:
   ```sh
   python bot.py

### 4. **Answering Questions**:
   - The bot will ask you a series of questions based on the selected question categories.
   - Speak your answer clearly into the microphone, and the system will process the speech using the **Google Speech Engine** (or the **eSpeak** engine if running on a Raspberry Pi).
   - The answers will be evaluated using NLP techniques, keyword matching, and fuzzy matching.

### 5. **Generating Results**:
   After completing the interview or viva session, the bot will generate a **results sheet** containing the answers and marks of the student/candidate. The results will be displayed on the terminal, and a CSV file will be generated for record-keeping. The file will be saved as `results.csv` in the project directory.

### 6. **Database and Question Bank Management**:
- The bot allows **teachers/interviewers** to add, update, and manage questions in the database for future interviews/vivas.
- The question bank supports questions of varying difficulty levels (easy, medium, hard) and question types (MCQs, fill-in-the-blanks, true/false, one-word answers).
- This ensures the bot remains flexible and relevant for different examination scenarios.


### **Future Work**

ViQu has a great future scope due to the vast application areas of the individual techniques used for making it, and some of those applications are mentioned below:

1. **Interview Bot:**
   Interviews are not just about the domain knowledge but are also about body language and the ability to work under pressure. By adding a camera and a deep learning model, ViQu could evaluate these aspects of the candidate.

2. **Non-Technical Interviews:**
   Not just technical interviews, but by applying machine learning, deep learning, and semantic analysis, non-technical interviews may also be conducted, eliminating the need for human interviewers during the entire process.

3. **Interview/Viva for Non-Objective Questions:**
   By using semantic analysis, ViQu could be extended to handle subjective questions in interviews/vivas, such as essay-type answers, and evaluate them accordingly.

4. **Stress Management:**
   Beyond the technical field, ViQu could be used in psychology and mental health assessments. By integrating machine learning and semantic analysis, the bot could assess the stress level of candidates and provide tips on reducing stress if the levels are found to be above a certain threshold.
```

### **License**

This project is not licensed. All rights reserved.
