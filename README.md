# Noor – AI-Powered Arabic Language Tutor for Autistic Children

Noor is an AI-powered interactive Arabic tutor designed to support language practice and social engagement for children with Autism Spectrum Disorder in Arabic-speaking communities.

The project combines Arabic speech interaction, computer vision, an animated face interface, and physical movement through a hybrid edge-cloud architecture.

## Prototype

![Noor prototype](noor-prototype.jpg)

## Key Features

- Arabic speech interaction using STT, LLM, and TTS
- Face tracking and child localization
- Emotion-aware interaction
- Animated face with idle, listening, and speaking states
- Servo-based head movement toward the child
- Smart interruption when the child starts speaking
- Hybrid edge-cloud processing

## System Architecture

```text
Child
  |
  v
Camera + Microphone
  |
  v
NVIDIA Jetson
Tracking + VAD + Control
  |
  v
Cloud AI
Groq Whisper -> Gemini -> ElevenLabs
  |
  v
Speaker + Animated Face + Servo Motion
```

Local processing handles real-time sensing, tracking, motion, and visual interaction, while cloud AI services handle Arabic speech transcription, language reasoning, and speech synthesis.

## Hardware

- NVIDIA Jetson AGX Xavier
- ZED 2 Camera
- ReSpeaker USB Mic Array V3.1
- Arduino Uno
- Servo motors
- Display and speaker
- LM2596 DC-DC converters

## Technologies

- Python
- OpenCV
- WebRTC VAD
- PyTorch / ONNX
- Arduino C/C++
- Groq Whisper API
- Gemini API
- ElevenLabs API
- Computer Vision
- Speech Processing
- Edge-Cloud Integration

## Project Presentation

The repository includes a short graduation-defense presentation:

[Noor Project Presentation](Noor_Project_Presentation.pdf)

The presentation gives a high-level overview of the project. This README summarizes additional technical details from the full project documentation.

## Repository Files

- `Noor_Project_Presentation.pdf`
- `noor-prototype.jpg`
- `README.md`

## Source Code

The source code is intentionally not included in this public repository.

## Author

**Mohammad Ahmad Elayyan**

- Email: [mohamadelayyan84@gmail.com](mailto:mohamadelayyan84@gmail.com)
- LinkedIn: https://www.linkedin.com/in/mohammadelayyan1
- GitHub: [MohammadElayyan117](https://github.com/MohammadElayyan117)
