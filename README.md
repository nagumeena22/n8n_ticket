🤖 AI-Powered IT Ticket Routing Workflow

This project is an automated helpdesk workflow built using n8n.
It receives support requests from multiple channels, uses AI to classify them, and routes each ticket to the correct team automatically.

🚀 Overview

The workflow acts as an intelligent ticket triage system that:

Accepts tickets from chat, web forms, and email

Normalizes incoming data into a standard format

Uses AI to classify ticket category and priority

Routes tickets to the appropriate Slack channel

Sends a confirmation email to the requester

🏗 Architecture Flow
Input → Normalize → AI Classify → Parse → Route → Notify → Confirm
📥 Input Channels

The system supports:

Chat interface trigger

Web form submission trigger

Gmail trigger (incoming emails)

All inputs are transformed into a unified ticket structure before processing.

🧠 AI Classification Layer

An AI Agent analyzes the ticket content and determines:

Category (Hardware, Software, Network, Access, etc.)

Priority

Structured summary

Structured output parsing ensures the response is valid JSON and prevents formatting errors.

🔀 Intelligent Routing

A Switch node routes tickets based on AI classification:

Hardware → Hardware Team (Slack)

Software → Software Team (Slack)

Network → Network Team (Slack)

Access → Access Team (Slack)

📢 Notifications

Each team receives a Slack notification.

The requester receives an automated confirmation email.

✅ Key Benefits

Reduces manual ticket triage

Improves response time

Eliminates routing errors

Scales support operations

Enhances user experience

🛠 Technologies Used

n8n (Workflow Automation)

OpenAI / Gemini Chat Model

Slack Integration

Gmail Integration

Structured Output Parser

🎯 Use Case

Ideal for IT departments or support teams looking to automate ticket intake and routing using AI-driven classification.
