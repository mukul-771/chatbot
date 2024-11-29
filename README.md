# AI Voice Chat

An interactive voice chat application that enables real-time conversations with an AI assistant using OpenAI's APIs. The application supports voice input, text processing, and voice output, creating a natural conversation flow with the AI.

## Features

- 🎤 Real-time voice recording
- 🔄 Speech-to-text conversion using OpenAI's Whisper API
- 💭 AI-powered responses using GPT-3.5 Turbo
- 🔊 Text-to-speech output using OpenAI's TTS API
- 💾 Conversation history tracking
- ⌨️ Simple keyboard controls

## Prerequisites

- Node.js (v14 or higher)
- FFmpeg
- OpenAI API key
- Working microphone and speakers

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd ai-voice-chat
```

2. Install dependencies:
```bash
npm install
```


3. Create a `.env` file based on `.env.example`:

```bash
cp .env.example .env
```


4. Add your OpenAI API key to the `.env` file:
```bash
OPENAI_API_KEY=your_openai_api_key_here
```

## Usage

1. Start the application:

```bash
node ttsChat.js
```
or
```bash
OPENAI_API_KEY=your_openai_api_key_here node ttsChat.js
```



2. Controls:
- Press `Enter` to start recording
- Press `Enter` again to stop recording and process your message
- Press any other key to exit
- Use `Ctrl+C` to force quit

## Dependencies

- `node-microphone`: For audio input
- `fluent-ffmpeg`: For audio processing
- `ffmpeg-static`: FFmpeg binaries
- `axios`: For API requests
- `speaker`: For audio output
- `openai`: OpenAI API client
- `dotenv`: Environment variable management
- `form-data`: For handling multipart form data

## Configuration

The application uses several configurable parameters:

- Voice Settings:
  - Default voice: "echo"
  - TTS model: "tts-1"
- Chat Model: GPT-3.5 Turbo
- Audio Settings:
  - Channels: 2 (Stereo)
  - Bit Depth: 16
  - Sample Rate: 44100 Hz

## Limitations

- Audio file size limit: 25MB for Whisper API
- Requires a stable internet connection
- OpenAI API usage is subject to API pricing

## Error Handling

The application includes error handling for:
- Microphone recording issues
- API communication errors
- Audio processing problems


## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

