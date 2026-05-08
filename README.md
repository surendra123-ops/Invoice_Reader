# Invoice Information Extractor 📄

Deploy  Link: https://inovicesreader.streamlit.app/#extracted-text

This is a simple AI-powered Invoice Information Extractor project built using Streamlit, OCR, and Groq LLM.

The application allows users to upload invoice images and automatically extracts important invoice details like:

* Invoice Number
* Date
* Vendor Name
* Total Amount
* GST Details
* Other invoice information

The extracted information is converted into structured JSON format using AI.

---

# Features 🚀

* Upload invoice images
* Extract text using OCR (Tesseract)
* Process invoice data using LLM
* Convert invoice data into JSON format
* Download extracted JSON file
* Simple and clean Streamlit UI

---

# Tech Stack 🛠️

* Python
* Streamlit
* Tesseract OCR
* LangChain
* Groq API
* Llama3 Model
* Pillow
* dotenv

---

# Project Flow 📌

```text id="1m3hq2"
Invoice Image
     ↓
OCR Text Extraction
     ↓
Groq LLM Processing
     ↓
Structured JSON Output
```

---

# Project Structure 📂

```text id="dyvfev"
project/
│
├── app.py
├── requirements.txt
├── packages.txt
├── .env
└── README.md
```

---

# Installation ⚙️

## Clone Repository

```bash id="l9j9a4"
git clone <your-repository-link>
cd project-folder
```

---

## Create Virtual Environment

### Windows

```bash id="9flr0z"
python -m venv venv
venv\Scripts\activate
```

### Linux/Mac

```bash id="mnv06r"
python3 -m venv venv
source venv/bin/activate
```

---

# Install Requirements

```bash id="wk0t9x"
pip install -r requirements.txt
```

---

# Install Tesseract OCR

## Windows

Download and install Tesseract OCR:

[Tesseract OCR Installer](https://github.com/UB-Mannheim/tesseract/wiki?utm_source=chatgpt.com)

After installation add this line in `app.py`:

```python id="jlwmk0"
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

---

# Add Environment Variable

Create `.env` file:

```env id="zjx00i"
GROQ_API_KEY=your_api_key
```

Get Groq API Key from:

[Groq Console](https://console.groq.com?utm_source=chatgpt.com)

---

# Run Project ▶️

```bash id="6gq5m7"
streamlit run app.py
```

Application will run on:

```text id="lj7m1m"
http://localhost:8501
```

---

# Sample Output 📋

```json id="jlwmk1"
{
  "invoice_number": "INV-101",
  "date": "08-05-2026",
  "vendor_name": "ABC Pvt Ltd",
  "total_amount": "₹5000"
}
```

---

# Future Improvements 🔥

* PDF Invoice Support
* Multi-language OCR
* Export to Excel/CSV
* Database Integration
* Dashboard Analytics
* FastAPI Backend Integration

---

# About Project 👨‍💻

This project was developed as a beginner-friendly AI/LLM application to understand:

* OCR processing
* AI-based information extraction
* LangChain integration
* LLM structured output generation
* Streamlit deployment

---


