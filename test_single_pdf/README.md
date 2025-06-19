# 📄 OCR PDF Project (Thai-English)

## 🎯 Purpose  
This project is designed to extract text from PDF files using Optical Character Recognition (OCR), supporting both Thai and English languages. It automatically detects whether a PDF page is text-based or image-based, cleans the extracted text, and extracts key fields such as Study ID, Visit, PID, Fixed ID, and Initials using regular expressions.

---

## ⚙️ Features
- Supports both text-based and image-based PDF files
- Uses PyMuPDF and pdf2image to process PDF pages
- Integrates Tesseract OCR with Thai and English language support
- Cleans and formats extracted text
- Extracts structured data using regular expressions
- Saves results to a `.txt` file

---

## 🚀 Usage
1. Connect to Google Drive to access PDF files  
2. Use `ocr_pdf_return_text()` to extract text from PDF  
3. Clean the text using `clean_ocr_text()`  
4. Extract key fields using `extract_fields_from_text()`  
5. Save the results to a `.txt` file and download

---

## 🧪 Example Output
```json
{
  "Study": "ABC123",
  "Visit": "Visit 1",
  "PID": 123456,
  "Fixed ID": "F123-456",
  "Initials": "XYZ"
}

