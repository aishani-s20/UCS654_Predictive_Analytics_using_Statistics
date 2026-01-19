# TOPSIS: Algorithm, Package & Web Application

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![PyPI](https://img.shields.io/badge/PyPI-Package-green?style=for-the-badge&logo=pypi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

---

## 📑 Assignment Summary
This repository acts as a consolidated portfolio for the **Predictive Analysis** assignment. It demonstrates the implementation of the **Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS)** method across three progressive stages: mathematical scripting, library distribution, and web-based deployment.

### 🔗 Quick Access Guide

| Task ID | Project Module | Key Functionality | Resource Link |
| :---: | :--- | :--- | :---: |
| **1** | **Local Script** | Command-line tool for local data processing. | [📂 Source Code](https://github.com/aishani-s20/TOPSIS_Implementation) |
| **2** | **PyPI package** | Installable package hosted on PyPI. | [📦 Package Repo](https://github.com/aishani-s20/TOPSIS_PYPI) |
| **3** | **Web Interface** | Interactive GUI with email automation. | [🌐 Web App Repo](https://github.com/aishani-s20/TOPSIS_Web_App) |

---

## 💡 Implementation Details

### 🔹 Part 1: Mathematical Implementation (CLI)
A standalone Python utility designed to perform multi-criteria decision-making analysis on CSV datasets.
* **Core Logic:** Implements vector normalization, ideal best/worst identification, and Euclidean distance calculation.
* **Error Handling:** Includes strict checks for file existence, column consistency, and non-numeric data types.
* **Execution Command:**
    ```bash
    python topsis.py <InputFile.csv> <Weights> <Impacts> <OutputFile.csv>
    ```
    *Sample:* `python topsis.py data.csv "0.25,0.25,0.25,0.25" "+,+,-,+" ranking.csv`

### 🔹 Part 2: PyPI Package
The core algorithm has been modularized and published to the Python Package Index, allowing for global accessibility and easy integration into other projects.
* **Library Name:** `TOPSIS-Aishani-102303250`
* **Installation Method:**
    ```bash
    pip install TOPSIS-Aishani-102303250
    ```
* **Registry Link:** [View on PyPI.org](https://pypi.org/project/TOPSIS-Aishani-102303250/)

### 🔹 Part 3: TOPSIS Web Service
A user-friendly web application built with Streamlit that removes the need for coding knowledge. This service processes data and delivers results asynchronously.
* **Capabilities:**
    * Drag-and-drop CSV upload.
    * Dynamic input fields for weights and impacts.
    * **Automated Emailing:** Results are sent directly to the user's provided email address via SMTP.
* **Live Deployment:** [Launch Application](https://topsiswebapp.streamlit.app/)

---

## 🧰 Development Stack
* **Core Language:** Python 3.x
* **Data Processing:** Pandas, NumPy
* **Web Framework:** Streamlit
* **Automation:** smtplib (Email Protocol)

---

## 🎓 Student Details
**Submitted by:** Aishani Shreya  
**Roll Number:** 102303250  
**Course:** UCS654 Predictive Analytics using Statistics  
**Institute:** Thapar Institute of Engineering & Technology


---

