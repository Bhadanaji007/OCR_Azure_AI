# OCR_Azure_AI

This project uses **Azure Cognitive Services – Vision API** to extract text from images using Optical Character Recognition (OCR). It is implemented in Python with the official Azure AI SDK (`azure-ai-vision-imageanalysis`), and configured via a `.env` file.

---

## 📌 Features

- Uses Azure's `imageanalysis` SDK to extract printed text
- Simple CLI script to analyze images
- Secure key + endpoint management via `.env`
- Designed for labs, demos, and fast OCR experimentation

---

## 🛠️ Setup Instructions (All Steps in One)

### ✅ 1. Clone the Repository

bash
git clone https://github.com/Bhadanaji007/OCR_Azure_AI.git
cd OCR_Azure_AI
✅ 2. Create Virtual Environment & Activate It
python -m venv labenv
# For Linux/macOS:
source labenv/bin/activate
# For Windows PowerShell:
.\labenv\Scripts\Activate.ps1
✅ 3. Install Dependencies
pip install -r requirements.txt
pip install azure-ai-vision-imageanalysis==1.0.0
✅ 4. Create .env File with Your Azure Keys
code .env  # or use nano .env

Paste the following content into .env and replace with your real Azure values:

VISION_KEY=your_azure_vision_key
VISION_ENDPOINT=https://<your-endpoint>.cognitiveservices.azure.com/

You can find these in the Azure Portal > Cognitive Services > Keys and Endpoint.

Run the OCR Script

python read-text.py
