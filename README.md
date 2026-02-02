# TRP 1 — MCP Setup Challenge (Tenx MCP + VS Code)

This repository documents my completion of the **TRP 1 — MCP Setup Challenge**, including Tenx MCP server setup, AI agent rule configuration, and insights from testing AI-assisted development workflows.

---

## Project Overview

The goal of this challenge is to verify my ability to:

* Configure a modern MCP-enabled coding environment
* Connect the **Tenx MCP Analysis Server**
* Improve AI agent behavior using structured rules
* Document insights about human–AI collaboration

---

## Task 1 — Tenx MCP Setup (VS Code)

### Steps Completed

1. Updated **VS Code** to the latest version
2. Installed required extensions:

   * GitHub Copilot
   * GitHub Copilot Chat
3. Created MCP configuration file:

```
.vscode/mcp.json
```

### MCP Server Configuration

```json
{
  "servers": {
    "tenxfeedbackanalytics": {
      "url": "https://mcppulse.10academy.org/proxy",
      "type": "http",
      "headers": {
        "X-Device": "linux",
        "X-Coding-Tool": "vscode"
      }
    }
  },
  "inputs": []
}
```

4. Connected MCP server in **Copilot Chat → Agent Mode**
5. Authenticated MCP server via GitHub
6. Confirmed MCP tools are active and logging interactions

---

## Task 2 — AI Agent Rules Configuration

### Rules File Location

```
.github/copilot-instructions.md
```

### Key Improvements Added

* Clear communication standards for the AI agent
* Step-by-step reasoning enforcement
* Anti-hallucination safeguards
* Debugging and troubleshooting expectations
* Alignment with my workflow and decision-making

### Purpose

These rules improve:

* AI clarity
* Output accuracy
* Collaboration quality
* Predictability of responses

---

## Task 3 — Testing AI Agent Behavior

### What Worked Well

* Agent responses became more structured
* Better adherence to instructions
* Reduced irrelevant or speculative answers
* Improved problem-solving transparency

### Challenges Encountered

* Initial MCP connection setup
* Understanding MCP server authentication flow
* Fine-tuning instruction strictness

### Troubleshooting Actions

* Re-checked MCP JSON formatting
* Restarted MCP server and VS Code
* Adjusted rule verbosity for balance

---

## Key Insights Gained

* AI agent behavior is **strongly shaped by rules**
* Clear constraints reduce hallucinations and noise
* Explicit instructions improve consistency and alignment
* MCP enables measurable insight into AI–developer collaboration

---

## Repository Structure

```
.github/copilot-instructions.md   # AI Agent Rules
.vscode/mcp.json                  # MCP Server Config
docs/mcp-report.md               # Challenge Documentation
README.md                         # Project Overview
```

---

## Submission Notes

* MCP connection remained active throughout the challenge
* This repository contains all required artifacts
* Demonstrates technical comprehension, curiosity, and AI workflow experimentation
