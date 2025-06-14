# 🔊 Text-to-Voice API (Spring Boot + Vosk TTS Integration)

This project is a **Java-based Text-to-Speech (TTS)** REST API built with **Spring Boot**. It takes **text input** and returns **spoken audio output**, with plans to support **local Zambian languages** like **Bemba**.

---

## 🚀 Features

* ✅ Convert plain text into spoken audio
* 🔊 Output audio using tools like `espeak`, `flite`, or other TTS engines
* 🌐 REST API endpoint for text-to-voice conversion
* 💬 Designed to support **local languages** with future custom voice models
* 📱 Backend-ready for a voice-assist mobile app (e.g., for farmers)

---

## 🛠️ Tech Stack

* **Java 17+**
* **Spring Boot**
* **Maven**
* **TTS Engine**: `espeak`, `flite`, or custom wrapper
* (Optional) **Vosk for STT** — for future speech recognition support

---

## 📁 Project Structure

```
text_to_voice/
├── src/
│   ├── main/
│   │   ├── java/com/nextinnomind/text_to_voice/  ← Java source code
│   │   └── resources/                            ← Spring config
│   └── test/                                     ← Unit tests
├── models/                                       ← (Optional) Vosk models folder
├── .gitignore
├── pom.xml                                       ← Maven config
└── README.md
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/SilasChalwe/text_to_voice.git
cd text_to_voice
```

### 2. Build the project

```bash
./mvnw clean install
```

### 3. Run the application

```bash
./mvnw spring-boot:run
```

### 4. Test the API

Send a request using Postman or Curl:

```http
POST /api/text-to-speech
Content-Type: application/json

{
  "text": "Hello, welcome to the voice service!"
}
```

🔊 The API will generate and play the audio or return a file (depending on implementation).

---

## 📦 Future Plans

* Train and add **Bemba or Nyanja TTS voices**
* Flutter frontend integration
* Speech-to-Text using [Vosk](https://alphacephei.com/vosk/) (future)
* Save generated audio to local disk or cloud storage

---

## 📜 License

MIT License — free to use, modify, and contribute.

---

## 👤 Author

**Silas Chalwe**
🔗 GitHub: [@SilasChalwe](https://github.com/SilasChalwe)
