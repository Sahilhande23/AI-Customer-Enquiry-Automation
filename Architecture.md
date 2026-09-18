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
Gmail
   ↓
Customer

## Process

1. Customer sends an enquiry.
2. n8n Webhook receives the request.
3. AI analyzes the enquiry and generates a response.
4. Customer details and AI response are stored in Google Sheets.
5. The generated response is returned to the customer.
6. The AI-generated reply is automatically sent to the customer's email using Gmail.
## Data Flow

## Input

Customer sends:
- Name
- Email
- Enquiry message

Example:

{
  "name": "Sahil",
  "email": "sahil@example.com",
  "message": "Hello, I want information about your product."
}

## Processing

1. Webhook receives customer enquiry
2. AI analyzes the enquiry
3. AI generates a suitable response
4. Customer data and AI response are stored in Google Sheets
5. AI response is automatically sent to the customer through Gmail

## Output

- AI-generated customer reply
- Customer enquiry stored in Google Sheets
- Automatic email sent to customer
- JSON response returned through Webhook
