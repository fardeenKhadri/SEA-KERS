# SPOOKY- Smart Personalized Outreach & Optimized Kare for You

## Overview
This project demonstrates real-time audio and video streaming using Python and Google Gemini AI for generating responses. It utilizes `asyncio`, `pyaudio`, and `opencv` for handling input/output operations.

## Features
- Captures and streams audio and video from the default input devices.
- Sends text input to the AI model for processing.
- Handles real-time AI responses, including text and audio.
- Plays back generated audio responses.

## Prerequisites
- Python 3.11+
- Required Python packages:
  ```sh
  pip install asyncio pyaudio opencv-python pillow google-generativeai
  ```
- Google Gemini AI API key (replace `YOUR_API_KEY_HERE` in the code).

## Usage
1. Clone the repository and navigate to the project directory.
2. Install dependencies.
3. Run the script:
   ```sh
   python script.py
   ```
4. Enter messages in the console to interact with the AI.
5. Press `q` to exit.

## Notes
- This is for demonstration purposes only. Do not use for production without proper modifications.
- Ensure your microphone and webcam are accessible by the script.

## License
This project is for educational purposes only and should not be used commercially without permission.

