# Wealthfront Incident Management GPT - Configuration

> **Demo Project:** Created for an OpenAI AI Deployment Manager application. Not affiliated with or endorsed by Wealthfront Corp. or Notion Labs, Inc.

## Overview

This repository contains all configuration files needed to build a Custom GPT that automates incident post-mortem documentation. The GPT integrates with Notion's API to generate structured reports through natural conversation.

## Live Demo

- **Custom GPT:** [Incident Post-Mortem Pam](https://chatgpt.com/g/g-68f13fbab7dc8191a3034d506d02d2fd-incident-post-mortem-pam)
- **Notion Workspace:** [Wealthfront Incident Post-Mortems](https://drt-cloud.notion.site/Wealthfront-Incident-Post-Mortems-28d868965b3880f2b8bdd103d2500a7f)

## Repository Contents

```
wealthfront-incident-gpt-demo/
├── README.md
├── instructions.txt          # Complete GPT system prompt
├── custom_action.yaml        # Notion API OpenAPI schema
└── knowledge/                # Knowledge files that are uploaded to the CustomGPT
    ├── knowledge_file_example_1.md
    └── knowledge_file_example_2.md
```

## What Each File Does

**`instructions.txt`**
- Holds the instructions used within the CustomGPT

**`custom_action.yaml`**
- OpenAPI 3.1.0 schema for Notion integration
- API endpoints for search and page creation
- Authentication configuration

**`knowledge/`**
- Files that are uploaded to the CustomGPT for additional knowledge

## How It Works

1. **Interview:** User describes new incident → GPT asks clarifying questions
2. **Generate:** GPT creates structured post-mortem page in Notion automatically

## Quick Start

1. Set up a Notion workspace with Knowledge Base and Incidents database
2. Create Notion API integration and copy token
3. Go to [ChatGPT GPT Editor](https://chat.openai.com/gpts/editor)
4. Copy `instructions.txt` → Paste as Instructions
5. Upload files from `knowledge/` → Add to Knowledge
6. Import `custom_action.yaml` → Add as Action
7. Configure Bearer auth with your Notion API token

**Authentication:** Bearer token (Notion integration token)

## Contact

**Jeret Shuck**
- Email: jeret.shuck@gmail.com
- LinkedIn: [linkedin.com/in/jeret-shuck](https://www.linkedin.com/in/jeretshuck15963/)
- Created: October 2025

---

**Disclaimer:** This is a demonstration project created for an OpenAI job application. Not affiliated with Wealthfront Corp. or Notion Labs, Inc. All trademarks belong to their respective owners.
