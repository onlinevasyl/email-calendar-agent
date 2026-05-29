# Setup Guide: Email & Calendar Events Agent

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
