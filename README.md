# Wealthfront Incident Management GPT - Configuration

> **Demo Project:** Created for an OpenAI AI Deployment Manager application. Not affiliated with or endorsed by Wealthfront Corp. or Notion Labs, Inc.

## Overview

This repository contains all configuration files needed to build a Custom GPT that automates incident post-mortem documentation. The GPT integrates with Notion's API to search past incidents and generate structured reports through natural conversation.

## Live Demo

- **Custom GPT:** [LINK_TO_GPT]
- **Notion Workspace:** [LINK_TO_NOTION_PAGE]
- **Demo Video:** [LINK_TO_VIDEO]

## Repository Contents

```
wealthfront-incident-gpt-demo/
├── README.md
├── instructions.txt          # Complete GPT system prompt
├── custom_action.json        # Notion API OpenAPI schema
└── knowledge/                # Knowledge files that are uploaded to the CustomGPT
    ├── knowledge_file_1.md
    └── knowledge_file_2.md
```

## What Each File Does

**`instructions.txt`**
- Holds the instructions used within the CustomGPT

**`custom_action.json`**
- OpenAPI 3.1.0 schema for Notion integration
- API endpoints for search and page creation
- Authentication configuration

**`knowledge/`**
- Files that are uploaded to the CustomGPT for additional knowldge

## How It Works

1. **Search:** User asks about past incidents → GPT searches knowledge base
2. **Interview:** User describes new incident → GPT asks clarifying questions
3. **Generate:** GPT creates structured post-mortem page in Notion automatically

## Quick Start

1. Set up a Notion workspace with Knowledge Base and Incidents database
2. Create Notion API integration and copy token
3. Go to [ChatGPT GPT Editor](https://chat.openai.com/gpts/editor)
4. Copy `instructions.txt` → Paste as Instructions
5. Upload files from `knowledge/` → Add to Knowledge
6. Import `custom_action.json` → Add as Action
7. Configure Bearer auth with your Notion API token

## Value Proposition

**Why use a GPT for incident documentation?**
- Natural language input (no rigid forms)
- Intelligent follow-up questions
- Searches institutional knowledge automatically
- Consistent formatting and structure
- 75% estimated time reduction vs manual documentation

**Authentication:** Bearer token (Notion integration token)

## Use Case: Wealthfront

Digital wealth management platform requiring rapid, consistent incident documentation for:
- Site Reliability Engineers (incident response)
- Engineering Managers (trend analysis)
- Compliance Team (audit requirements)

## Contact

**Jeret Shuck**
- Email: jeret.shuck@gmail.com
- LinkedIn: [linkedin.com/in/jeret-shuck]
- Created: October 2025

---

**Disclaimer:** This is a demonstration project created for an OpenAI job application. Not affiliated with Wealthfront Corp. or Notion Labs, Inc. All trademarks belong to their respective owners.
