Intelligent Structured Document Data Extraction System

Project Description

The Intelligent Structured Document Data Extraction System is a UiPath automation built using Document Understanding to extract key information from different types of structured documents automatically. The bot processes documents such as resumes, invoices, bank statements, purchase orders, and order forms, identifies their type, extracts predefined fields, and stores the extracted data in Excel. This automation reduces manual work and improves accuracy and efficiency in document processing.


How It Works

The project follows a Dispatcher–Performer architecture.

The Dispatcher reads documents from a folder and sends each file as a transaction to a UiPath Queue. Each queue item contains details such as file path, file name, and received time.

The Performer processes each transaction by classifying the document type and extracting the required data fields. After extraction, successfully processed files are moved to the Processed folder, while files with errors are moved to the Unprocessed folder. Finally, all extracted data is written to an Excel file for reporting.

Extracted Fields

Resume

1. Name
2. Email
3. Date of Birth
4. Phone Number
5. LinkedIn

Order Form

1. OrderName
2. OrderDate
3. CustomerName
4. Total Amount

Bank Statement

1. AccountNumber
2. TransactionDate
3. StatementDate
4. TransactionAmount
5. Balance

Purchase Order

1. PONumber
2. PODate
3. VendorName
4. Total Amount
 
Invoice

1. Billed To
2. Invoice Number
3. Due Date
4. Date of issue
5. Amount Due 

Date of Issue

Amount Due
