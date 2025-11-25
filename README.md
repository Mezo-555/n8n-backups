# n8n Workflow Backups 🤖

This repository acts as an automated "Time Machine" for my self-hosted n8n instance.

## 🚀 How it works
This backup process is handled by a specialized n8n workflow that calls the n8n Public API to:
1.  **Fetch** all workflows from the server.
2.  **Compare** the current version with the saved version.
3.  **Commit** any changes or new workflows to this repository as `.json` files.

## 📂 Structure
Workflows are stored in the `workflows/` directory, organized by creation date:
`workflows/YYYY/MM/workflow-id.json`

## 🔄 Automation
The backup workflow runs automatically on a daily schedule to ensure no logic is ever lost.
