🤖 AI Agent – Automated Customer Feedback Handler (n8n)
📌 Overview

This project is an AI-powered Customer Feedback Agent built in n8n to reduce manual effort in sorting and managing customer feedback.

Instead of a person manually checking every feedback and forwarding it to the right team, this agent automatically classifies, routes, and responds to feedback in real-time.

⚡ How It Works

Form Trigger – The workflow starts when a customer submits the feedback form.

LLM Classification – An AI model (Google Gemini) analyzes the feedback and categorizes it as:

Complaint

Feature Request

Compliment

Routing via Switch Node – Based on classification:

Complaint → Sent to the complaints department (via Airtable + Slack) + acknowledgement email to the customer.

Feature Request → Sent to the product team + confirmation email to the customer.

Compliment → Sent to the owner’s department + thank-you email to the customer.

Automated Notifications – Customers instantly get a tailored response via Gmail.

🛠️ Tools & Integrations

n8n (workflow automation)

Google Gemini LLM (classification)

Airtable (feedback storage)

Slack (team notifications)

Gmail (automated customer replies)

🎯 Benefits

Eliminates manual sorting of feedback

Ensures instant acknowledgement to customers

Routes issues and suggestions to the right team without delay

Boosts efficiency and customer experience

📂 Repository Contents

customer-feedback-form.json → n8n workflow file

Documentation for setup and usage

Example emails and Slack messages

🚀 Getting Started

Import the JSON workflow into your n8n instance.

Configure credentials for Airtable, Slack, and Gmail.

Connect your form to trigger the workflow.

Activate and let the AI Agent handle customer feedback automatically.

🔮 Future Enhancements

Multi-language feedback support

Sentiment analysis for deeper insights

Dashboard for analytics and tracking
