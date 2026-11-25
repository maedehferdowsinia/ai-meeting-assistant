# AI Meeting Assistant

An AI-powered meeting assistant built with n8n, OpenAI, and Didar CRM.

This workflow automates the process of collecting meeting information, transcribing audio, generating structured meeting documents, and syncing meeting records with a CRM system.

Overview

The AI Meeting Assistant helps businesses turn meeting conversations and notes into structured, actionable documents.

Users interact with the assistant through the Bale messenger. The workflow collects meeting audio and additional information, processes the content using AI, generates a Word document, and optionally registers the meeting in Didar CRM.

"Workflow Overview" (assets/workflow-overview.png)

Key Features

- Conversational Data Collection: Collects meeting audio, notes, customer name, mobile number, and meeting details through Bale.
- AI Audio Transcription: Converts meeting audio into text using OpenAI.
- AI-Powered Content Processing: Analyzes meeting information and generates structured content.
- Multiple Output Types: Generates meeting minutes or business proposals based on the selected output type.
- Word Document Generation: Creates formatted ".docx" files.
- CRM Integration: Finds or creates customer records and registers meeting activities in Didar CRM.
- Automated File Attachment: Attaches generated meeting documents to CRM activities.
- Conversation State Management: Uses n8n Data Tables to manage multi-step conversations.

Workflow Architecture

1. Input: Receives user messages and meeting information through a Bale webhook.
2. Data Collection: Guides the user through submitting audio, notes, customer details, and meeting preferences.
3. Audio Processing: Downloads and transcribes the submitted audio.
4. AI Processing: Combines the transcription and additional notes to generate the requested output.
5. Document Generation: Creates a formatted Word document.
6. CRM Synchronization: Creates or finds the customer and registers the meeting activity in Didar CRM.
7. Delivery: Sends the generated document and response back through Bale.

Tech Stack

- n8n – Workflow automation and orchestration
- OpenAI – Audio transcription and AI-powered content generation
- Bale Messenger API – User interaction and message delivery
- Didar CRM – Customer and meeting activity management
- n8n Data Tables – Conversation state and meeting data storage
- JavaScript – Data processing and document generation

Requirements

To run the workflow, you need:

- An n8n instance
- A Bale bot and bot API token
- OpenAI API credentials
- Didar CRM API credentials
- The required Didar CRM community node for n8n
- Configured n8n Data Tables

Setup

1. Download the workflow JSON file from this repository.
2. Import it into your n8n instance.
3. Configure the required credentials for OpenAI and Didar CRM.
4. Set your Bale bot token and configure the webhook URL.
5. Create and configure the required Data Tables and replace the placeholder table IDs.
6. Configure the required Didar CRM IDs and other environment-specific settings.
7. Activate the workflow and test the conversation flow.

Important: This repository contains a sanitized workflow template. Credentials, API tokens, webhook addresses, and environment-specific IDs must be configured before execution.

Security Notice

Never commit API tokens, passwords, private webhook URLs, customer information, or real meeting recordings to a public repository.

Project Status

Workflow implementation completed. Deployment requires environment-specific configuration and testing.

---

Learning Outcomes & Career Direction

Building this project has been a practical step toward my goal of working in AI Engineering, particularly in AI-powered systems and intelligent automation.

Through this project, I gained hands-on experience in:

- Designing multi-step AI-powered workflows.
- Integrating LLMs and external APIs into business processes.
- Building stateful conversational systems.
- Connecting AI solutions with CRM platforms.
- Transforming unstructured meeting data into structured business outputs.
- Developing practical AI solutions around real-world business needs.

This project has strengthened my interest in AI Systems Engineering, AI Solutions Development, and AI Product Development, while providing a foundation for exploring more advanced AI/ML applications.
