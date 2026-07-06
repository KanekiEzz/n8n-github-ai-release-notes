# GitHub AI Release Notes Bot

An automated n8n workflow that generates AI-powered release notes from GitHub commits using Google Gemini and sends them directly to Discord.

This repository is sanitized for sharing. The workflow uses placeholder values for credentials, repository owner/repo, and Discord webhook URL.

## Preview

![Workflow Preview](images/demo.gif)

## Features

- GitHub Push Trigger
- Fetch Commit Details
- AI Release Notes (Gemini 2.5 Flash)
- Discord Notifications
- Zero manual work

## Workflow

GitHub Push
↓
HTTP Request
↓
Gemini AI
↓
Discord Webhook

## Technologies

- n8n
- GitHub API
- Google Gemini
- Discord Webhooks

## Installation

1. Import the workflow into n8n.
2. Replace placeholder values in the workflow JSON:
	- `YOUR_GITHUB_OWNER`
	- `YOUR_GITHUB_REPO`
	- `YOUR_WEBHOOK_ID`
	- `YOUR_WEBHOOK_TOKEN`
3. Configure GitHub credentials in n8n and attach them to GitHub nodes.
4. Configure Gemini API credentials in n8n and attach them to the Gemini node.
5. Activate the workflow.

## Security

- Never commit real webhook URLs, API keys, credential IDs, or instance IDs.
- Keep secrets in n8n credentials or environment variables.

## License

MIT