                                                            Inya Buildathon 2025

Executive Summary:

This project suggests a Conversational AI Banking Support Agent. The agent is capable of interacting with
customers via voice or chat, process regular questions like account balance, transaction history,
card blocking, and escalate to a human agent when appropriate.

Architecture

The system design consists of the following elements:
- NLU (Natural Language Understanding): Intents and entity extraction.
- Dialog Manager: Conversation flow and decision management.
- API Layer: Integration with mock banking services.
- Mock Datastore: Customer, account, and transaction data storage.
- Escalation Module: Passes unresolved inquiries to human representatives.

Data Schemas

Schema definitions are as follows:
- Customer (ID, name, contact, accounts)
- Account (ID, type, balance, status)
- Transaction (ID, account, date, type, amount)
- Escalation Ticket (ID, intent, status, assigned agent)
- FAQ / Knowledge Base (intents, sample questions, answers)

 Demo Videos
 
 - Balance Inquiry → [YouTube Link]
 - Card Blocking → [YouTube Link]
 - Escalation → [YouTube Link]

 Setup Instructions
 
 This is a no-code design project. Everything is documented within this PDF. The repository contains
 supporting files: Architecture Diagram, Data Schemas, API Documentation, and Test Results
 Summary. 

 API Stubs
 
 - GET /balance/:customer_id → Returns account balance
 - GET /transactions/:account_id → Returns last N transactions
 - POST /block-card → Creates a block-card reques

Test Results Summary
Scenario                          Result
 
- Balance Inquiry             -      PASS
- Transaction History         -      PASS
- Card Blocking               -      PASS
- Escalation to Human Agent   -      PASS


  
