
---

```markdown
#  Grammar Scoring Engine

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)

A voice analysis tool that evaluates grammatical correctness in spoken responses, developed for SHL's Research Intern position.

---

## 🚀 Features

- 🎤 Audio recording directly in the notebook  
- 🔊 Speech-to-text conversion  
- 🔍 Grammar error detection and highlighting  
- 📊 Scoring system (0-100 scale)  
- 📝 Detailed error explanations with suggestions  

---

## 📦 Requirements

- Python 3.8+
- Jupyter Notebook
- Microphone (for recording)

---

## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone [repository-url]
   cd grammar-scoring-engine
   ```

2. Install dependencies:
   ```bash
   pip install language-tool-python pyaudio SpeechRecognition
   ```

---

## 🧪 Usage

1. Open `SHL_Grammar_Scoring_Engine.ipynb` in Jupyter Notebook  
2. Run all cells sequentially  
3. When prompted:
   - Speak clearly into your microphone
   - The system will record for 5 seconds  
4. View results:
   - ✅ Transcribed text  
   - 📈 Grammar score  
   - 🟡 Highlighted grammar issues  
   - 💡 Correction suggestions  

---

## 💡 Sample Output

```
Transcribed Text: He go to school everyday

Grammar Score: 80/100
Corrected Text: He [[go→goes]] to school everyday

Error Details:
1. At position 3:
   Error: 'go'
   Suggested: ['goes']
   Rule: ENGLISH_SIMPLE_REPLACE
```

---

## 🧠 Technical Approach

### 🎙️ Audio Processing
- PyAudio for real-time audio recording  
- Google Speech Recognition API for transcription

### ✏️ Grammar Analysis
- LanguageTool for error detection
- Custom scoring algorithm based on error severity and frequency

### 📊 Visualization
- IPython for real-time audio playback
- Color-coded highlighting for detected grammar issues

---

## 🛠️ Troubleshooting

- **Microphone Not Detected**  
  Ensure your system microphone is enabled and accessible by Python

- **Speech Recognition Fails**  
  Check your internet connection — Google API requires it

- **PyAudio Installation Issues (esp. on macOS/Linux)**  
  You may need system packages:
  ```bash
  # For Ubuntu/Debian
  sudo apt-get install portaudio19-dev python3-pyaudio
  ```

- **Permission Errors in Notebook**  
  Restart the kernel and re-run all cells

---

## 📸 Demo

![Notebook Screenshot](assets/notebook_example.png)

---

## 🌱 Future Enhancements

- Integration with SHL's assessment rubrics  
- Advanced fluency and coherence metrics  
- Support for domain-specific vocabulary  

---

