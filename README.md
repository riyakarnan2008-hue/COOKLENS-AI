CookLens AI

CookLens AI is an OCR-powered cooking assistant built with Python, Streamlit, OpenCV, and Tesseract OCR. It extracts recipe and cooking-related text from uploaded images and presents the detected information in a clean and readable format.

The project demonstrates how Computer Vision and Optical Character Recognition (OCR) can be applied to make recipe information easier to access and process.

Features

- 📷 Upload recipe or cooking-related images
- 🔍 Extract text using Tesseract OCR
- 🖼️ Image preprocessing using OpenCV
- 📝 Display extracted recipe text
- 🥕 Identify and organize cooking-related information
- 📋 Clean and readable output through Streamlit
- ⚡ Simple and interactive web interface
- 💻 Runs locally using Python

Technology Stack

Technology| Purpose
Python| Core programming language
Streamlit| Web application interface
OpenCV| Image processing and preprocessing
Tesseract OCR| Text recognition from images
Pytesseract| Python interface for Tesseract
NumPy| Image and numerical processing
PIL| Image handling

How It Works

User Uploads Image
        ↓
   Image Processing
        ↓
    OpenCV
        ↓
  Tesseract OCR
        ↓
   Text Extraction
        ↓
 Recipe Information
        ↓
 Streamlit Interface

Project Structure

CookLens-AI/
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── assets/
    └── sample-images/

Installation

1. Clone the Repository

git clone https://github.com/your-username/CookLens-AI.git

2. Navigate to the Project Folder

cd CookLens-AI

3. Create a Virtual Environment

python -m venv venv

4. Activate the Virtual Environment

Windows:

venv\Scripts\activate

macOS/Linux:

source venv/bin/activate

5. Install Dependencies

pip install -r requirements.txt

Tesseract OCR Setup

CookLens AI requires Tesseract OCR to recognize text from images.

After installing Tesseract, configure its executable path in "app.py" if required.

Example for Windows:

pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"

Make sure the path matches the location of Tesseract on your system.

Run the Application

Start the Streamlit application using:

streamlit run app.py

The application will open in your browser.

Usage

1. Launch CookLens AI.
2. Upload a recipe or cooking-related image.
3. The image is processed using OpenCV.
4. Tesseract OCR detects the text.
5. Extracted information is displayed through the Streamlit interface.
6. Review the recipe and cooking instructions.

Example Use Cases

CookLens AI can be useful for:

- 📖 Digitizing printed recipes
- 🥗 Extracting ingredients from recipe images
- 🍲 Reading cooking instructions
- 📝 Converting recipe images into editable text
- 📱 Processing recipes captured using a mobile camera
- ♻️ Reducing manual typing of recipe information

OCR Processing

The application uses image preprocessing techniques to improve OCR accuracy.

Typical processing includes:

Input Image
     ↓
Resize / Convert
     ↓
Grayscale
     ↓
Noise Reduction
     ↓
Thresholding
     ↓
Tesseract OCR
     ↓
Extracted Text

The quality of the input image can affect OCR accuracy. Clear, well-lit images with readable text generally produce better results.

Requirements

Example "requirements.txt":

streamlit
opencv-python
pytesseract
numpy
Pillow

Future Enhancements

- 🤖 AI-based recipe summarization
- 🥕 Automatic ingredient detection
- 📊 Nutritional information analysis
- 🌐 Multi-language OCR support
- 🔊 Text-to-speech recipe instructions
- ⏲️ Automatic cooking timer generation
- 🛒 Automatic shopping-list generation
- 💡 Recipe recommendations based on available ingredients

Advantages

- Simple and user-friendly interface
- Reduces manual recipe transcription
- Combines OCR with computer vision
- Easy to run locally
- Useful real-world application of AI and image processing
- Can be extended with additional AI capabilities

Limitations

- OCR accuracy depends on image quality.
- Handwritten text may not be recognized accurately.
- Complex backgrounds can affect text detection.
- Tesseract must be installed separately on the system.

License

This project is developed for educational and project demonstration purposes.

Author

Riya

CookLens AI — An OCR-powered approach to making cooking information easier to read, extract, and use.