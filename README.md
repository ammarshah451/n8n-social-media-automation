# n8n Social Media Automation Workflow

This n8n workflow automates the process of posting scheduled content to social media platforms.

## Workflow Overview

This automation workflow performs the following steps:

1. **Fetches Scheduled Posts from Google Sheets** - Retrieves upcoming posts from a Google Sheets document containing scheduled social media content

2. **Pre-Post Notification on Slack** - Sends a notification to Slack before posting to inform the team about the upcoming post

3. **Platform Selection & Posting** - Uses a switch case to determine the target platform and posts content to:
   - Discord (based on switch case condition)
   - Other social media platforms as configured

4. **Confirmation Message on Slack** - Sends a final confirmation message to Slack once the post has been successfully published

## Features

- Centralized content scheduling via Google Sheets
- Team notifications before and after posting
- Conditional platform routing with switch case logic
- Slack integration for workflow transparency

## Requirements

- n8n instance (self-hosted or cloud)
- Google Sheets API access
- Slack workspace and webhook/bot configuration
- Discord webhook or bot token
- Properly configured credentials in n8n

## Setup

1. Import the workflow into your n8n instance
2. Configure credentials for:
   - Google Sheets
   - Slack
   - Discord
3. Update the Google Sheets document ID and range
4. Set up Slack channel webhooks
5. Configure Discord webhook URLs
6. Adjust the switch case conditions as needed

## Usage

The workflow can be triggered manually or scheduled to run at specific intervals to check for and post scheduled content automatically.
