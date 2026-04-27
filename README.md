# 🎵 Random Sound Song Maker

A fun, interactive web application that lets users create music by recording sounds and generating random musical sequences. Perfect for 8th-grade students to experiment with music creation!

## Features

- **Record Sounds** - Capture 1-second audio clips directly from your microphone
- **Assign Sounds to Keys** - Each recorded sound is automatically saved to sequential keys (1, 2, 3, etc.)
- **Play Sounds** - Press number keys (1–9) on your keyboard to play the corresponding recorded sounds
- **Generate Random Songs** - Click "Generate Song" to create a random 20-note pattern using your recorded sounds, played back at 300ms intervals

## How to Use

1. Click the **"Record Sound"** button to start recording a new sound (records for 1 second)
2. Each sound is automatically assigned to the next available key
3. Press number keys **1–9** to play back your recorded sounds in real-time
4. Click **"Generate Song"** to create and play a random musical sequence using all your recorded sounds

## Technical Details

- Built with vanilla JavaScript and the Web Audio API
- Uses `navigator.mediaDevices.getUserMedia()` to capture audio from the user's microphone
- Uses `MediaRecorder` API to process and store audio clips as `Blob` objects
- Stores sounds as `Audio` objects indexed by key numbers
- Generates random patterns by selecting from available recorded sounds

## Requirements

- Modern web browser with microphone access permission
- JavaScript enabled
- HTTPS connection (required for `getUserMedia` API in production)

## Files

- `index.html` - Complete application (HTML + CSS + JavaScript)

Enjoy creating music! 🎶
