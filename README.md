# 📝 Meeting Minutes LLM Transcriber

This project leverages state-of-the-art Large Language Models (LLMs) and speech-to-text technology to convert meeting audio recordings into concise, structured meeting minutes. It uses **OpenAI Whisper** for transcription and **Meta's LLaMA 3.1-8B-Instruct** for summarization.

## 🔧 Features

- 🎙️ Audio transcription using `whisper-1` model (OpenAI)
- 🧠 Summarization using Meta's LLaMA 3.1-8B-Instruct
- 📦 Runs on Google Colab with easy setup
- 🔐 HuggingFace token integration
- 💾 Audio file loading from Google Drive

## 🚀 Getting Started

### 1. Clone this repository

```bash
git clone https://github.com/your-username/meeting-minutes-llm-transcriber.git
cd meeting-minutes-llm-transcriber
```

### 2. Open in Google Colab

Upload the `meeting_minutes.ipynb` notebook to your Google Drive, or open it directly in Colab.

### 3. Setup Environment

The notebook handles installation of the following dependencies:

- `transformers`
- `torch`
- `openai`
- `bitsandbytes`
- `accelerate`
- `httpx==0.28.1`

### 4. Authentication

You'll need:

- OpenAI API key (for Whisper)
- Hugging Face token (for LLaMA model access)

### 5. Add Your Audio File

Mount Google Drive and provide the path to your `.mp3` file:

```python
drive.mount("/content/drive")
audio_filename = "/content/drive/MyDrive/your-folder/your-meeting.mp3"
```

## 🧪 Model Details

- **Whisper-1**: OpenAI's general-purpose speech recognition model.
- **Meta LLaMA 3.1-8B-Instruct**: Lightweight yet powerful model for summarization and dialogue generation.

## 📄 Output

The final output is a clean, formatted summary of the meeting content suitable for sharing or storing as official meeting minutes.

## 📌 TODOs

- Add UI for uploading audio files
- Add support for diarization (speaker identification)
- Export summaries to PDF or Markdown

## 📜 License

MIT License

## 🙌 Acknowledgements

- OpenAI Whisper
- Meta LLaMA 3
- Hugging Face Transformers

Built with 💡 by Trisham Bharat Patil
