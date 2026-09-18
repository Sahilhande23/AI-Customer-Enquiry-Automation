# System Architecture

## Workflow

Customer
   ↓
Webhook
   ↓
AI Response Generator
   ↓
Google Sheets
   ↓
Respond to Webhook

## Process

1. Customer sends an enquiry.
2. n8n Webhook receives the request.
3. AI analyzes the enquiry and generates a response.
4. Customer details and AI response are stored in Google Sheets.
5. The generated response is returned to the customer.

## Data Flow

Input:
- Customer Name
- Email
- Message

Output:
- AI Generated Reply
- Customer information stored in Google Sheets
