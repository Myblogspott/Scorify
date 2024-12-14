# Scorify
### `README.md` for **Scorify**

---

# Scorify

**Scorify** is an AI-powered application designed to assist users with interactive learning, test preparation, and real-time question detection. Built with cutting-edge AI integrations, Scorify offers multiple features like **Interactive Reading**, **Interactive Listening**, and **OTP Validation** for secured access.

---

## **Features**

### 1. **OTP Validation (index.html)**
- Users can securely validate OTPs with a responsive and user-friendly interface.
- Automatically handles OTP input transitions between fields.
- Includes real-time countdown for OTP expiry and displays expiration alerts.
- API integration for OTP validation ensures secure authentication.
- **Action on Success**: Redirects users to the main application after successful OTP validation.

---

### 2. **Interactive Reading (interactive_reading.html)**
- Enables text detection from uploaded images or live camera feed using **Google Vision API**.
- Extracted text is processed via **OpenAI GPT-4 fine-tuned models** for generating accurate answers.
- Perfect for practicing tests like **Duolingo** or similar reading exercises.
- **Key Functionalities**:
  - Upload an image or start a live video feed.
  - Extract and analyze text in real time.
  - Generate responses strictly based on the text with no unnecessary context.
  - Speak out the answers for user convenience.

---

### 3. **Interactive Listening (interactive_listening.html)**
- Records user audio and processes the topic to generate insights or hints for improvement.
- Provides a **"Listen and Speak"** functionality where the user speaks about a topic, and hints are generated in real-time using GPT.
- **Unique Features**:
  - **Hint Generation**: AI listens to the spoken content and provides topic-specific hints.
  - Detects text under the camera to match with the spoken topic and generate the best possible answers.
  - Users can practice **summarization skills** with prompts like: *"Summarize the topic into 75 seconds for the camera."*
  - **Speaking Sample Support**: Assists in recording practice answers for speaking tests.

---

### 4. **Live Feed AI (livefeed.html)**
- Acts as a hub for all Scorify functionalities.
- Options to:
  - Start a live camera feed for text detection.
  - Access **Interactive Reading** and **Interactive Listening** modules.
  - Record topics and generate responses or summaries.
- Fully interactive design for seamless transitions between modules.

---

## **Core Functionalities**
1. **AI-Powered Text Detection**:
   - Utilizes **Google Vision API** for extracting text from images or video feeds.
   - Processes text dynamically to generate meaningful and context-based answers.

2. **Speech Recognition**:
   - Implements browser-based **SpeechRecognition API** for real-time transcription.
   - Records and processes user speech to generate hints or summarize conversations.

3. **Audio Output**:
   - Uses `speechSynthesis` to provide audio responses for answers, summaries, or hints.

4. **Dynamic Hint Generation**:
   - Context-based hint generation using **GPT-4 fine-tuned models**.
   - Supports dynamic prompts to help users refine their responses.

---

## **How to Run the Application**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/scorify.git
   cd scorify
   ```

2. Host the application:
   - Use any hosting service like **Netlify**, **Vercel**, or a local server.
   - For local testing, use:
     ```bash
     python -m http.server
     ```

3. Open the application in your browser:
   - Navigate to `http://localhost:8000` (if using Python server).

---

## **Technology Stack**
- **Frontend**: HTML5, CSS3, JavaScript (ES6), Bootstrap 5.
- **APIs**:
  - **Google Vision API** for text detection.
  - **OpenAI GPT-4** for answer generation and hint creation.
- **Browser APIs**:
  - `SpeechRecognition` for audio transcription.
  - `SpeechSynthesis` for text-to-speech responses.

---

## **File Structure**
```
scorify/
│
├── index.html                 # OTP Validation Page
├── interactive_reading.html   # Interactive Reading Module
├── interactive_listening.html # Interactive Listening Module
├── livefeed.html              # Main Hub for Scorify Features
├── assets/                    # Static assets (images, styles, etc.)
├── scripts/                   # Additional JavaScript files (if any)
└── README.md                  # Documentation for the app
```

---

## **How to Use Scorify**

1. **Step 1**: Access the **Live Feed App** (livefeed.html):
   - Choose **Interactive Reading** to practice text-based exercises.
   - Choose **Interactive Listening** to practice speaking and summarization.

2. **Step 2**: Enable Camera and Microphone:
   - Grant camera permissions for text detection.
   - Grant microphone permissions for speech recognition.

3. **Step 3**: Practice & Get Feedback:
   - Generate AI-based hints for better learning.
   - Summarize conversations and refine your understanding.

---

## **API Configuration**
1. Replace the placeholder `YOUR_GOOGLE_CLOUD_API_KEY` in the script sections with your **Google Vision API Key**.
2. Replace the placeholder `YOUR_OPENAI_API_KEY` in the script sections with your **OpenAI API Key**.

---

## **Future Enhancements**
- Offline support using **Service Workers**.
- Integration with user profiles for personalized feedback.
- Expansion to include multi-language support for global users.

---

### **Credits**
- **Frontend Framework**: [Bootstrap](https://getbootstrap.com/)
- **APIs**: [Google Cloud Vision](https://cloud.google.com/vision), [OpenAI GPT](https://platform.openai.com/)
- **Icons**: [Bootstrap Icons](https://icons.getbootstrap.com/)

Happy Learning with **Scorify**! 🚀
