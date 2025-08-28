
# Voice Assistant with Face Unlock

This project is a **Python-based Voice Assistant** with an added **Face Recognition Unlock System**.
It combines **speech recognition, text-to-speech, chatbot responses, web automation, and computer vision** into one assistant, similar to J.A.R.V.I.S.

---

## Features

* **Face Unlock System**

  * Uses OpenCV and LBPH face recognizer.
  * Collects and trains face data.
  * Unlocks assistant only for authorized users.

* **Voice Assistant Functionalities**

  * Greets user based on the time of day.
  * Responds to basic conversations.
  * Provides the current time.
  * Shuts down system with a command.
  * Enters "sleep mode" and wakes up only after recognizing the user’s face.

* **Web Automation**

  * Google Search via voice commands.
  * YouTube search and playback.
  * Opens websites like YouTube, Google, WhatsApp Web, Spotify, GitHub.

* **Chatbot Responses**

  * Small talk such as greetings, asking assistant’s name, creator, etc.

---

## Technologies Used

* **Python 3**
* **Libraries:**

  * `speech_recognition` → For voice input.
  * `pyttsx3` → For text-to-speech.
  * `opencv-python` (`cv2`) → For face detection & recognition.
  * `numpy` → For face training.
  * `Pillow (PIL)` → For image processing.
  * `webbrowser` → To open websites.
  * `datetime`, `os`, `random` → Utility functions.

---

## Project Structure

VoiceAssistant
│── assistant.py          # Main Python script
│── trainer.yml           # Face recognizer trained model (auto-generated)
│── face_dataset/         # Stored face samples
│── README.md             # Project documentation

---

## Setup & Installation

1. **Clone this repository**

   git clone https://github.com/Debojeet-ops/voice-assistant.git
   cd voice-assistant

2. **Install dependencies**

   pip install opencv-python opencv-contrib-python numpy pillow pyttsx3 SpeechRecognition

3. **Run the assistant**

   python assistant.py

---

## Usage

1. When you start, the assistant says:
   **"I am your voice assistant. Show me your face to start."**

2. **Face Unlock**

   * If it’s your first run, it collects face data and trains the recognizer.
   * On later runs, it verifies your face to unlock.

3. **Available Commands**

   * "Hello" → Greets you.
   * "What is the time?" → Tells current time.
   * "Search Google for <query>" → Opens Google search.
   * "Search YouTube for <query>" / "Play on YouTube <query>" → Plays YouTube video search.
   * "Open YouTube / Google / WhatsApp / Spotify / GitHub" → Opens site.
   * "Shutdown" → Shuts down the system.
   * "Exit" or "Stop" → Puts assistant in sleep mode (reactivates with face).

---

## Notes

* Press **Q** while collecting/training faces to stop early.
* At least **30 face samples** are recommended for good accuracy.
* Works best in **good lighting conditions**.

---

## Future Improvements

* Add **multi-user support** (different users can train their faces).
* Add **voice authentication** along with face recognition.
* Improve chatbot with **NLP models** for better responses.
* Integrate with **smart home devices**.

---

## Author

**Debojeet Adhikari**
| AI Enthusiast | Python Developer | Tech Explorer

