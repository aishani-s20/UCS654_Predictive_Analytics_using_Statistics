# 🎵 YouTube Audio Mashup Suite

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Streamlit](https://img.shields.io/badge/Built%20With-Streamlit-ff4b4b.svg)
![FFmpeg](https://img.shields.io/badge/Audio-FFmpeg-green.svg)
![yt-dlp](https://img.shields.io/badge/Downloader-yt--dlp-yellow.svg)
![Status](https://img.shields.io/badge/Project-Active-success.svg)

| Version | Repository Link | Application |
|---------|----------------|------------------|
| **CLI Version** | [Song_Mashup_CLI](https://github.com/aishani-s20/Song_Mashup_CLI) | (Local Terminal) |
| **Web Service** | [Song_Mashup_Web_Service](https://github.com/aishani-s20/Song_Mashup_Web_Service) | [Mashup Pro Live](https://mashuppro.streamlit.app/) |

---

## 📘 Project Overview

This suite provides a **dual-approach** to generating high-quality musical mashups. Whether you prefer the control of a local terminal or the convenience of a cloud-based web app, this toolkit automates the fetching, trimming, and merging of audio tracks into a single MP3.

### 🔹 Core Logic & Workflow

Both versions share a robust backend designed for musical quality:

* **Smart Filtering:** Automatically skips files longer than 15 minutes to avoid non-music content.
* **Intelligent Trimming:** Each track is cut starting at the 21-second mark to ensure intros and silence are removed.
* **Seamless Merging:** Snippets are concatenated using `pydub` into a high-quality 192kbps MP3.

---

## 🖥️ 1. Command-Line Interface (CLI)

Designed for local automation and power users who need granular control over file naming and local storage.

### 📖 Usage Format

Run the script from your terminal using the following positional arguments:

```bash
python 102303250.py <SingerName> <NumberOfVideos> <AudioDuration> <OutputFileName>
```

### 💡 Examples:

* **Standard Mashup:** 
  ```bash
  python 102303250.py "Javed Ali" 11 25 my_mashup.mp3
  ```

### ✅ Validation:

Enforces a minimum of **11 videos** and **21-second snippets** to ensure a professional "mashup" feel.

---

## 🌐 2. Streamlit Web Service

A cloud-optimized version designed for maximum uptime and zero local configuration.

### 🚀 Key Features:

* **Reliability Fix:** While YouTube often blocks data center IPs (like Streamlit Cloud), this version utilizes **SoundCloud** as a primary source to ensure 100% download success.
* **Automated Delivery:** No manual downloads; the app zips the mashup and sends it directly to your provided email address via secure SMTP. 📧
* **UI/UX:** Features a centered **"Orange Ombre"** theme with a custom glassmorphism design. 🎨

### 🔗 Access the Web App:

👉 [https://mashuppro.streamlit.app/](https://mashuppro.streamlit.app/)

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **yt-dlp** | For high-speed audio extraction |
| **Pydub** | For precise audio manipulation and merging |
| **Streamlit** | For the responsive web interface |
| **FFmpeg** | The underlying engine for audio processing (managed via `packages.txt` on the web) |

---

## 📦 Installation (CLI Version)

### Prerequisites

Make sure you have **Python 3.9+** installed.

### Install Dependencies

```bash
pip install yt-dlp pydub static-ffmpeg
```

**Note:** This tool uses `static-ffmpeg` to handle audio conversions, so you don't need to manually install FFmpeg on your system.

---

## 🎯 Comparison: CLI vs Web Service

| Feature | CLI Version | Web Service |
|---------|------------|-------------|
| **Platform** | Local Terminal | Cloud (Streamlit) |
| **Audio Source** | YouTube | SoundCloud (primary) |
| **Output Delivery** | Local file | Email (ZIP) |
| **Setup Required** | Yes (dependencies) | No |
| **Customization** | High | Medium |
| **Reliability on Cloud** | N/A | Optimized ✅ |

---

## 👤 Author Details

**Aishani Shreya**

- **Roll Number:** 102303250
- **Institute:** Thapar Institute of Engineering & Technology
- **GitHub:** [@aishani-s20](https://github.com/aishani-s20)
- **Email:** aishani1020@gmail.com

---

⭐ **If you found these tools helpful, please consider starring the repositories!**
