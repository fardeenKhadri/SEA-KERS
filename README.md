# **SPOOKY: Smart Personalized Outreach & Optimized Kare for You**
SPOOKY is an **AI-powered real-time assistant** that integrates **WebRTC, WebSockets, and Google Gemini AI** to provide **voice and video-based assistance**.

## **Features**
✅ **Live Video Processing** - Captures video frames and sends them to the AI for analysis.  
✅ **Voice Control with Toggle** - Enables AI-powered voice interactions.  
✅ **WebSocket-Based Communication** - Real-time data exchange between frontend and backend.  
✅ **Neon-Themed UI** - Futuristic **black & neon blue** interface.  

---

## **Project Structure**
```
/spooki_project
│── index.html                # Main frontend UI (WebRTC, WebSocket, and UI elements)
│── main.py                   # WebSocket server (Google Gemini integration)
│── pcm-processor.js          # Web Audio API worklet for processing PCM data
│── README.md                 # Project documentation
```

---

## **Installation & Setup**
### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/spooky-ai.git
cd spooky-ai
```

### **2. Install Dependencies**
Ensure you have **Python 3.8+** installed.

Install required Python packages:
```bash
pip install google-genai websockets asyncio
```

---


### **3. Start the WebSocket Server**
Run the WebSocket server:
```bash
python main.py
```
You should see:
```
BIFROST IS READY TO CONNECT ASGARD AND MIDGARD
```

---

### **4. Open the Frontend**
1. **Option 1:** Open `index.html` directly in a browser.
2. **Option 2:** Start a simple HTTP server:
   ```bash
   python -m http.server 6106
   ```
3. Open the browser and go to:
   ```
   http://localhost:6106/
   ```

---

## **How It Works**
### **WebRTC Camera Streaming**
- Captures **live video** from the webcam.
- Every **3 seconds**, a frame is converted to **base64** and sent to the **AI server**.
- The AI analyzes the frame and **returns text/audio responses**.

### **WebSockets Communication**
- The frontend **sends live audio & video** to the server.
- The AI processes **voice commands & images** and returns **real-time responses**.
- Responses are displayed in the **chat log** or **played as audio**.

### **Microphone Toggle for AI Voice Interaction**
- Toggle **ON** to **start voice processing**.
- Toggle **OFF** to **stop microphone input**.

---

## **Key Files**
### **1️⃣ index.html (Frontend)**
Contains:
- **WebRTC video streaming**
- **WebSockets integration**
- **Microphone toggle for AI interaction**

### **2️⃣ main.py (Backend WebSocket Server)**
- Receives **audio & video** from the frontend.
- Sends **AI-generated text & audio responses** back to the user.

### **3️⃣ pcm-processor.js (Audio Processing)**
- Uses **Web Audio API** to process **PCM audio data**.
- Ensures smooth **real-time voice communication**.

---

## **Usage Instructions**
1. **Run `main.py` to start the WebSocket server**.
2. **Open `index.html` in a browser**.
3. **Allow camera & microphone access**.
4. **Toggle the microphone ON** and start speaking.
5. **The AI will analyze video & voice input, responding accordingly**.

---

## **Troubleshooting**
### **WebSocket Not Connecting**
- Ensure the WebSocket server is running:
  ```bash
  python main.py
  ```
- Refresh the browser and try again.

### **No AI Response**
- Make sure your **Google API Key** is set up correctly.
- Check **server logs** for any errors.

### **Camera or Microphone Not Working**
- **Allow camera & microphone access** in browser settings.
- Restart your browser and reload the page.

---

## **Future Improvements**
✅ **WebRTC Peer-to-Peer Calling**  
✅ **AI-powered Object Detection in Video**  
✅ **Chat History & Voice Playback**  



---

## **License**
📜 **MIT License** - Free to use, modify, and distribute.  
