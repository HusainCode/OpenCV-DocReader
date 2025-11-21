# OpenCV-DocReader
Main hub repo for the DocReader platform.

Contains links to:
- DocReader-Training
- DocReader-Python-Service
- DocReader-CPP-Inference
- DocReader-WebUI

A simple document-scanning system that uses Machine Learning and Computer Vision to read documents, extract text, and pull important fields.  
The project will be trained and prototyped in **Python**, then deployed in **C++** for high performance.  
Data will be stored in **SQL**, and the full system may be containerized with **Docker**.

---

## ⭐ Features (Planned)

- Upload images or PDFs (receipts, invoices, checks, statements)
- Clean/prepare documents using OpenCV (deskew, denoise, threshold)
- OCR extraction (read text using Tesseract or custom models)
- Extract key fields (date, total, name, account number, etc.)
- Confidence scores for extracted fields
- Basic validation (date format, currency format, account number checks)
- Duplicate document detection
- Multi-language OCR support
- Save documents + extracted fields into SQL database
- Simple TypeScript/React frontend for uploading and viewing results
- Optional Docker setup for backend + database

---

## 🔧 Tech Stack

**Train / Logic (Python)**
- FastAPI or Flask for API
- OpenCV for preprocessing
- Tesseract / pytesseract for OCR
- Optional ML/ONNX models for field detection
- SQLAlchemy for database access

**High-Performance Deployment (C++)**
- OpenCV C++
- Tesseract C++ API
- Optional: ONNX model with OpenCV DNN
- Communicates with Python backend or runs as a standalone service

**Database**
- MySQL or MariaDB

**Frontend**
- TypeScript + React (or Next.js)

**Deployment**
- Docker (optional, recommended later)
- docker-compose for API + DB + C++ service

---

## 🚀 Basic Development Plan

1. **Python MVP**
   - Build upload API
   - Add basic OpenCV preprocessing
   - Add OCR with Tesseract
   - Return extracted text as JSON

2. **Field Extraction**
   - Add regex and simple rules
   - Parse date, total, vendor, etc.

3. **Frontend**
   - TypeScript upload form
   - Display raw text + extracted fields

4. **SQL Integration**
   - Save documents and results to MySQL

5. **C++ Version**
   - Rewrite preprocessing + OCR in C++
   - Add ONNX model support if used
   - Connect C++ engine to backend

6. **Docker (Optional)**
   - Container for Python API
   - Container for MySQL
   - Container for C++ service

---

## 📌 Status

Project is in the planning phase. Features and implementation details will be added as development progresses.

