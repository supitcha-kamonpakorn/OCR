# 📄 OCR PDF Batch Processor (Thai-English)

## 🎯 Purpose
This project is designed to extract text from **multiple PDF files** using Optical Character Recognition (OCR), supporting both Thai and English languages. It processes all PDF files in a specified folder, detects whether each page is text-based or image-based, performs OCR if needed, cleans the extracted text, and extracts key fields using regular expressions. The results are saved as JSON files per PDF.

---

## ⚙️ Features
- Batch processing of multiple PDF files from a folder
- Detects text-based vs image-based pages
- Uses PyMuPDF and pdf2image to render PDF pages
- Integrates Tesseract OCR with Thai and English language support
- Cleans and formats extracted text
- Extracts structured fields: Study, Visit, PID, Fixed ID, Initials
- Saves results as `.json` files in organized subfolders


---
## 🧪 Example Output (JSON)
```json
{
  "example.pdf": [
    {
      "Study": "ABC123",
      "Visit": "Visit 1",
      "PID": 123456,
      "Fixed ID": "F123-456",
      "Initials": "XYZ"
    },
    {
      "Study": "ABC123",
      "Visit": "Visit 2",
      "PID": 123456,
      "Fixed ID": "F123-456",
      "Initials": "XYZ"
    }
  ]
}
