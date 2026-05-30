# Setup Guide: Email & Calendar Events Agent


## 📑 Table of Contents

- 🤖 Configure the Copilot Studio Agent
- 🔧 Configure MCP Tools
- 🔌 Configure Connectors
- ⚙️ Configure Agent Tools
- 🎯 Configure Triggers
- 🧪 Test the Agent
- 🚀 Deploy the Agent
- 🧑‍💼 Use in Microsoft 365 Copilot
- ✅ Setup Complete
- 📚 Documentation References

## Overview
This guide walks you through setting up the Email & Calendar Events Agent in your environment.

## Prerequisites

### Required Accounts & Access
- **Microsoft 365 Account**: For Outlook email and Calendar access, MCP Servers connections, deployment to M365 Copilot and MS Teams channels
- **Microsoft Copilot Studio License**: For building and deploying the agent
- **Power Platform Admin Role Permissions**: for managing Power Platform solution, permissions to create connections for MCP Servers, Power Platform connectors
- **M365 Admin Role Permissions**: to allow adding agent to the Agents Store in MS Teams, M365 Copilot

## Installation & Configuration

### Step 1: Set Up Microsoft Copilot Studio
1. Navigate to [Copilot Studio](https://copilotstudio.microsoft.com/)
2. Create a new Agent in dedicated Power Platform solution
3. Name it "Email & Calendar Events Agent"
4. Configure the agent description
5. Choose Claude Sonnet 4.6 as agent's AI model
6. Set instructions (copy instructions from instructions.MD)

### Step 2: Configure Email & Calendar MCP Servers
1. In Copilot Studio, go to **Tools**
2. Add the **New tool**
3. Choose Model context protocol to filter available MCP Servers
4. Reference screenshots for MCP Servers names and configurations
5. Ensure you have proper permissions in your account to create connections for MCP Servers and enable MCP tools
6. Test connections to ensure proper access


---

## 🤖 Configure the Copilot Studio Agent

1. Open **Microsoft Copilot Studio**
2. Create a new agent:
   - **Name:** Email & Calendar Agent
   - **Description:** AI-powered assistant for managing emails and calendar events using MCP servers
3. Select the model (e.g., Claude Sonnet 4.6)
4. Add the agent instructions (see README or `docs/agent-instructions.md`)

### 📸 Agent Overview

![Agent Overview](screenshots/agent_overview screen.png)

![Agent Overview 2](screenshots/agent_overview screen_2.png)

---

## 🔧 Configure MCP Tools

Your agent uses MCP servers for email and calendar management.

### 📧 Email Management MCP Server

- Add tool → Model Context Protocol
- Connect to **Email Management MCP Server**
- Ensure authentication is configured

![Email MCP](screenshots/email-management_mcp_server.png)

---

### 📅 Meeting / Calendar MCP Server

- Add tool → Model Context Protocol
- Connect to **Meeting Management MCP Server**

![Calendar MCP](screenshots/meeting_management_mcp_server.png)

---

## 🔌 Configure Connectors

### Delete Calendar Events Connector

- Add custom connector or existing connector
- Configure permissions and authentication

![Delete Events Connector](screenshots/delete_calendar_events_connector.png)

---

## ⚙️ Configure Agent Tools

1. Navigate to **Tools section**
2. Add all MCP tools and connectors
3. Ensure tools are enabled

![Agent Tools](screenshots/agent_tools.png)

---

## 🎯 Configure Triggers

Define when your agent should act automatically.

- Set trigger conditions for:
  - Email processing
  - Calendar actions

![Trigger Config](screenshots/agent_trigger_config.png)

---

## 🧪 Test the Agent

1. Open the **Test panel**
2. Try sample prompts:
   - "Summarize my latest emails"
   - "Schedule a meeting for tomorrow"
   - "Delete my meeting at 3 PM"

![Agent Test](screenshots365 Copilot
3. Publish the agent

![Deployment Channels](screenshots/deployment_channels.png)

---

## 🧑‍💼 Use in Microsoft 365 Copilot

Once deployed, the agent can be accessed directly in M365 Copilot.

![M365 Copilot](screenshots/agent_in_m365_copilot.png)

![M365 Copilot 2](screenshots/agent_in_m365_copilot_2.png)

---

## ✅ Setup Complete

Your Email & Calendar Agent is now ready to:

- 📧 Manage and analyze emails  
- 📅 Create, update, and delete calendar events  
- 🤖 Execute actions using MCP tools  
- ⚡ Respond to natural language requests  

---

## 📚 Documentation References

### 🤖 Microsoft Copilot Studio

- Overview of Copilot Studio:  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/

- Building and managing agents:  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/authoring-first-bot

---

### 🔧 Model Context Protocol (MCP)

- MCP overview and concepts:  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/agent-extend-action-mcp

- Using MCP servers in AI workflows:  
  https://learn.microsoft.com/en-us/visualstudio/ide/mcp-servers

---

### 🔌 Connectors (Power Platform)

- Power Platform connectors overview:  
  https://learn.microsoft.com/en-us/connectors/

- Creating custom connectors:  
  https://learn.microsoft.com/en-us/connectors/custom-connectors/

---

### 🧑‍💼 Deployment & Channels

- Publishing Copilot Studio agents:  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/publication-fundamentals-publish-channels

- Microsoft Teams integration:  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/publication-add-bot-to-microsoft-teams

---

### ⚡ Additional Learning

- Copilot Studio tools & architecture:  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/tools-overview

- AI agent design best practices:  
  https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance-best-practices

---
