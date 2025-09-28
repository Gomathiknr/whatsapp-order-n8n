# WhatsApp Order Automation (n8n + Google Gemini + Google Sheets)

## 📌 Overview
This project is an **AI-powered WhatsApp chatbot workflow** built using **n8n**.  
It allows businesses to take customer orders directly via WhatsApp, check inventory, answer FAQs, and log orders in Google Sheets.

## 🚀 Features
- WhatsApp trigger to capture incoming customer messages.
- Google Gemini (via LangChain) for AI-powered understanding of queries.
- Google Sheets integration for:
  - ✅ Inventory lookup
  - ✅ Order logging
  - ✅ FAQ database
- Conversation memory for contextual responses.
- Automated confirmation messages to customers.

## 🛠️ Tech Stack
- n8n (workflow automation)
- LangChain + Google Gemini
- WhatsApp Business API
- Google Sheets

## ⚙️ Setup Instructions
1. **Export & Import Workflow**
   - Open n8n → Import → Upload `whatsapp_order.json`.

2. **Configure WhatsApp API**
   - Get WhatsApp Business API credentials (phone number, access token).
   - Add to your n8n credentials.

3. **Set Up Google Sheets**
   - Create a sheet with 3 tabs:
     - `Inventory`
     - `Orders`
     - `FAQ`
   - Share with your Google Service Account.
   - Add credentials in n8n.

4. **Configure Gemini API**
   - Create API key from Google AI Studio.
   - Add it in n8n under LangChain Gemini node.

5. **Test**
   - Send a message from WhatsApp to your bot.
   - Order is saved in Google Sheet, confirmation sent back.

## 📊 Workflow Structure
- **Trigger:** WhatsApp message
- **AI Agent:** LangChain + Gemini
- **Memory:** Conversation buffer
- **Actions:**
  - Get Inventory (Google Sheets)
  - Post Orders (Google Sheets)
  - Get FAQ (Google Sheets)

## 🙌 Author
- Built by [Your Name]
