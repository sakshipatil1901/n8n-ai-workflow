# Email Chat Assistant

## Overview

Email Chat Assistant is an AI-powered n8n workflow that automatically manages client communications using Google Gemini, Gmail, and Google Calendar.

The workflow retrieves client information, analyzes context using AI, and generates professional email responses or updates automatically.

## Features

* AI-powered email generation using Google Gemini
* Client information retrieval from Google Calendar
* Email retrieval from Gmail
* Context-aware conversations using memory
* Automated client update emails
* Professional email drafting and response generation

## Workflow Architecture

```text
Schedule Trigger
       │
       ▼
   AI Agent
       │
 ┌─────┼─────────────┐
 │     │             │
 ▼     ▼             ▼
Gemini Memory   Google Tools
Model           (Calendar)
 │
 ▼
Get Client Email
 │
 ▼
Send Update Message
```

## Components

### Schedule Trigger

Initiates the workflow automatically based on a configured schedule.

### AI Agent

Acts as the orchestrator and determines which tools to use for processing client requests.

### Google Gemini Chat Model

Provides natural language understanding and generates professional email content.

### Simple Memory

Maintains conversation context and previous interactions.

### Get Many Tools

Retrieves client-related events and information from Google Calendar.

### Get Client Email Tool

Fetches relevant client email information from Gmail.

### Send Update Message Tool

Sends AI-generated updates and responses directly to clients.


## Technologies Used

* n8n
* Google Gemini API
* Gmail API
* Google Calendar API
* AI Agent Framework
* Memory Management

## Workflow File

```text
Email Chat Assistant agent.json
```

## Setup

1. Import the workflow into n8n.
2. Configure Google Gemini credentials.
3. Configure Gmail credentials.
4. Configure Google Calendar credentials.
5. Activate the workflow.
6. Configure the schedule trigger.
7. Test the workflow execution.

## Example Scenario

1. Workflow starts automatically.
2. AI Agent retrieves client details.
3. Gemini generates a professional response.
4. Gmail sends the update email.
5. Conversation context is stored in memory.

## Author

Sakshi Patil
