# 📄 AI Invoice Processing Automation (n8n)

Automatically extract invoice data using Google Gemini AI and store the results in Google Sheets using an end-to-end n8n workflow.

---

## 🚀 Overview

This project automates invoice processing by combining **n8n**, **Google Drive**, **Google Gemini AI**, and **Google Sheets**.

When a new invoice is uploaded to Google Drive, the workflow automatically:

- Downloads the invoice
- Sends it to Google Gemini AI
- Extracts key invoice information
- Converts the AI response into structured JSON
- Stores the data in Google Sheets
- Logs any errors for monitoring and troubleshooting

---

## 🎯 Problem

Manual invoice processing is repetitive, time-consuming, and prone to human error.

Businesses often spend hours entering invoice information into spreadsheets or accounting systems.

This workflow eliminates manual data entry using AI-powered document extraction.

---

## 💡 Solution

The automation performs the following steps:

1. Detects new invoices uploaded to Google Drive.
2. Downloads the invoice file.
3. Sends the document to Google Gemini AI for analysis.
4. Extracts:
   - Invoice Number
   - Invoice Date
   - Vendor
   - Customer
   - Subtotal
   - Tax
   - Total
   - Currency
5. Parses the AI response into valid JSON.
6. Appends the extracted data to Google Sheets.
7. Logs processing errors when extraction fails.

---

## 🛠️ Tech Stack

- n8n
- Google Drive API
- Google Gemini AI
- Google Sheets API
- JavaScript

---

## 📋 Features

- ✅ Automated invoice detection
- ✅ AI-powered document understanding
- ✅ Structured JSON extraction
- ✅ Automatic spreadsheet updates
- ✅ Error logging
- ✅ Modular workflow design

---

## 🔄 Workflow

```text
Google Drive Trigger
        │
        ▼
Download Invoice
        │
        ▼
Google Gemini AI
        │
        ▼
Code Node (Parse JSON)
        │
        ▼
Google Sheets
        │
        ├── Success Log
        │
        └── Error Log
```

---

## 📊 Sample Output

| Invoice Number | Vendor | Customer | Total | Currency |
|----------------|---------|----------|--------|----------|
| INV-90210 | Apex Digital Studio | Mark Vance | 540.00 | USD |

---

## 📁 Project Structure

```text
AI-Invoice-Processing/
│
├── workflow.json
├── README.md
├── screenshots/
│   ├── 01-workflow.png
│   ├── 02-google-drive.png
│   ├── 03-gemini-output.png
│   ├── 04-google-sheets.png
│   └── 05-error-log.png
├── sample-data/
│   └── sample-invoice.pdf
└── LICENSE
```

---

## 📸 Screenshots

### Workflow

---<img width="1285" height="416" alt="Screenshot 2026-08-01 180023" src="https://github.com/user-attachments/assets/9769eba8-964b-4479-bfee-015a56edd240" />


### Google Drive Trigger

---<img width="1590" height="731" alt="Screenshot 2026-08-01 180037" src="https://github.com/user-attachments/assets/84a477a4-ed5a-4dc9-bfe9-87e7b7000412" />


### Gemini AI Extraction

---<img width="1903" height="897" alt="Screenshot 2026-08-01 180116" src="https://github.com/user-attachments/assets/28fcd67d-ae25-4821-83f7-4c53a8aa9838" />


### Google Sheets Output

---<img width="1918" height="910" alt="Screenshot 2026-08-01 180141" src="https://github.com/user-attachments/assets/b1b81100-f3c4-4323-8618-7fafc66d03fd" />


## 🚀 Future Improvements

- OCR support for scanned invoices
- Duplicate invoice detection
- Confidence score validation
- Approval workflow
- QuickBooks integration
- SAP integration
- Multi-currency support

---

## 💼 Skills Demonstrated

- Workflow Automation
- AI Integration
- Prompt Engineering
- API Integration
- JavaScript
- JSON Parsing
- Error Handling
- Google Workspace Automation
- Business Process Automation

---

## 📈 Business Impact

This workflow significantly reduces manual invoice processing time by automatically extracting structured data from invoices using AI. It improves accuracy, minimizes repetitive tasks, and enables finance teams to focus on higher-value work.

---

## 📄 License

This project is provided for educational and portfolio purposes.
