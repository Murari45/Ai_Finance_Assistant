AI Banking Assistant

A production-style AI-powered banking application built using React, Spring Boot, MySQL, and RAG (Retrieval-Augmented Generation). The project combines traditional banking operations with modern AI capabilities to provide intelligent financial insights and document-based question answering.

Project Objective

The goal of this project is to build a modern banking platform where users can:

Manage their bank account securely
Transfer funds
View transaction history
Analyze spending using AI
Upload banking documents
Ask questions about uploaded documents using RAG
Tech Stack
Frontend
React
React Router
Axios
Bootstrap / Material UI
Backend
Java 21
Spring Boot
Spring Security
JWT Authentication
Spring Data JPA
Maven
Database
MySQL
AI
Gemini API (or OpenAI API)
RAG
Apache PDFBox
ChromaDB (or PostgreSQL + pgvector)
Embedding Model
Retrieval-Augmented Generation
Tools
Git
GitHub
Docker
Postman
Features
Authentication
User Registration
Secure Login
JWT Authentication
Password Encryption (BCrypt)
User Profile
Banking
View Account Details
Balance Check
Transaction History
Fund Transfer
Beneficiary Management
Mini Statement
AI Banking Assistant

Ask natural language questions like:

How much did I spend on food last month?
Show my highest expense category.
What are my recurring payments?
Suggest ways to save ₹5000 this month.
How much salary did I receive this year?

The assistant analyzes transaction history and generates personalized financial insights.

RAG-Based Document Assistant

Users can upload:

Bank Statements
Loan Documents
Tax Documents
Credit Card Statements

Example questions:

Summarize this bank statement.
What is my EMI amount?
When is my next loan payment?
Explain this transaction.
What is the interest rate in this document?
System Architecture
React Frontend
        │
 REST API (HTTPS)
        │
Spring Boot Backend
        │
 ├── Authentication
 ├── Banking Services
 ├── AI Service
 ├── RAG Service
 │
 ├── MySQL
 └── ChromaDB
          │
     Gemini/OpenAI API
Project Structure
ai-banking-assistant/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── src/
│   │   ├── controller/
│   │   ├── service/
│   │   ├── repository/
│   │   ├── entity/
│   │   ├── dto/
│   │   ├── security/
│   │   ├── config/
│   │   ├── ai/
│   │   ├── rag/
│   │   └── util/
│   └── pom.xml
│
├── docs/
│
└── README.md
Development Roadmap (90 Days)
Phase 1
Project Setup
GitHub Repository
Spring Boot
React
MySQL Connection
Phase 2
Authentication
JWT
Spring Security
Phase 3
Banking APIs
Phase 4
React Dashboard
Phase 5
AI Assistant
Phase 6
RAG
Phase 7
Analytics Dashboard
Phase 8
Testing
Phase 9
Deployment
Planned APIs
Authentication
POST /api/auth/register

POST /api/auth/login
Account
GET /api/account

GET /api/account/balance

GET /api/account/transactions

POST /api/account/transfer
AI
POST /api/ai/chat
Documents
POST /api/documents/upload

POST /api/documents/chat
Database Tables
Users
Accounts
Transactions
Beneficiaries
Documents
Chat History
AI Workflow
User Question

↓

Fetch Transactions

↓

Generate Prompt

↓

Gemini/OpenAI

↓

Financial Insight
RAG Workflow
Upload PDF

↓

Extract Text

↓

Split into Chunks

↓

Generate Embeddings

↓

Store in Vector Database

↓

Similarity Search

↓

LLM

↓

Answer
Future Enhancements
Fraud Detection
Budget Planner
Investment Suggestions
Voice Assistant
OCR for Scanned PDFs
Multi-language Support
Financial Health Score
Personalized Savings Recommendations
Email Notifications
Spending Forecasts
Learning Outcomes

This project demonstrates practical experience with:

Java & Spring Boot
REST API Development
Spring Security & JWT
React
MySQL Database Design
AI & LLM Integration
Retrieval-Augmented Generation (RAG)
Vector Databases
Docker & Deployment
Clean Architecture
Git & GitHub Workflow