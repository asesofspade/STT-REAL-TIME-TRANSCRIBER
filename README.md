# STT-REAL-TIME-TRANSCRIBER

Records your voice directly from Google Colab and transcribes everything into a single text.

---

## How it works

The notebook has two cells. The first one installs the dependencies, the second one runs everything.

Once you run the second cell, it accesses your microphone through the browser and starts listening. It only records when it detects sound — if you're not talking, nothing gets saved. When you finish a sentence and go silent for about 2-3 seconds, it saves that as a clip and waits for the next one. Each clip is stored as `recording1`, `recording2`, and so on.

When you're done, click the "Transcribe All" button and it will transcribe every clip and put it all together into one single text.

---

## How to use it

1. Open the notebook in Google Colab
2. Run cell 1 to install dependencies
3. Run cell 2 and allow microphone access when the browser asks
4. Start talking — pausing for 2-3 seconds saves the current clip and starts waiting for the next one
5. Click "Transcribe All" when you're done

---

## Technologies

- **Whisper** — transcription model
- **JavaScript (browser)** — microphone access and voice activity detection
- **Python** — handles the recordings and runs the transcription pipeline
- **Google Colab** — no local setup needed
