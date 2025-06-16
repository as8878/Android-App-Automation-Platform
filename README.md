
# Android App Automation Platform
---
## 🔧 Features

*  End-to-end Android app automation
*  Task execution using natural language instructions
*  UI parsing with view hierarchy extraction
*  Screenshot-based state analysis
*  LLM-based decision making and planning
*  Supports both real devices and emulators via ADB
*  Built on top of [DroidBot](https://github.com/honeynet/droidbot)

---

## 🚀 Quick Start

### 1️⃣ Prerequisites

* Python (>=3.7)
* Java (for using DroidBot)
* Android SDK (ensure `platform-tools` is added to your PATH)
* A connected Android device or emulator via `adb`
* OpenAI / GPT API key (or compatible LLM API)

---

### 2️⃣ Installation

```bash
git clone https://github.com/YourUsername/Android-App-Automation-Platform.git
cd Android-App-Automation-Platform
pip install -e .
```

---

### 3️⃣ Dataset (Optional)

To experiment with real apps and task data:

* Download the dataset: [DroidTask Dataset](https://drive.google.com/file/d/1HcI3m3tLPaVr4aktvajBFur6zfULV0kh/view?usp=sharing)
* Follow the dataset folder structure as described in [About Dataset](#about-dataset)

---

### 4️⃣ Configuration

* Add your GPT API key to `tools.py`:

```python
os.environ['GPT_URL'] = 'your_gpt_api_key'
```

---

### 5️⃣ Run

```bash
droidbot -a <path/to/app.apk> -o <output/folder> -task "<your task description>" -keep_env -keep_app
```

You can also try the demo scripts provided in the `/scripts` folder.

---

## ⚠ Known Limitations

* Automation performance may vary depending on app complexity and LLM response randomness.
* ADB connection to host machine required (no standalone on-device mode).

---

## 🤝 Acknowledgements

* Built on top of [DroidBot](https://github.com/honeynet/droidbot)

---

## 🔬 Research Paper Reffered

For full system details, please refer to the paper:
**[Empowering LLM to use Smartphone for Intelligent Task Automation](https://arxiv.org/abs/2308.15272)**

---
